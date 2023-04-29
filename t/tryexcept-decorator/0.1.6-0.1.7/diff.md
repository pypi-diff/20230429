# Comparing `tmp/tryexcept_decorator-0.1.6.tar.gz` & `tmp/tryexcept_decorator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryexcept_decorator-0.1.6.tar", last modified: Sat Apr 29 12:47:25 2023, max compression
+gzip compressed data, was "tryexcept_decorator-0.1.7.tar", last modified: Sat Apr 29 12:48:46 2023, max compression
```

## Comparing `tryexcept_decorator-0.1.6.tar` & `tryexcept_decorator-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:47:25.957435 tryexcept_decorator-0.1.6/
--rw-rw-rw-   0        0        0     1094 2023-04-07 12:59:02.000000 tryexcept_decorator-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      448 2023-04-29 12:47:25.957435 tryexcept_decorator-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2822 2023-04-27 15:12:18.000000 tryexcept_decorator-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 12:47:25.957435 tryexcept_decorator-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-04-29 12:47:21.000000 tryexcept_decorator-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:47:25.926193 tryexcept_decorator-0.1.6/tryexcept_decorator/
--rw-rw-rw-   0        0        0       53 2023-04-29 12:17:21.000000 tryexcept_decorator-0.1.6/tryexcept_decorator/__init__.py
--rw-rw-rw-   0        0        0     4388 2023-04-29 12:17:10.000000 tryexcept_decorator-0.1.6/tryexcept_decorator/decorator.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:47:25.957435 tryexcept_decorator-0.1.6/tryexcept_decorator.egg-info/
--rw-rw-rw-   0        0        0      448 2023-04-29 12:47:25.000000 tryexcept_decorator-0.1.6/tryexcept_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-29 12:47:25.000000 tryexcept_decorator-0.1.6/tryexcept_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:47:25.000000 tryexcept_decorator-0.1.6/tryexcept_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-29 12:47:25.000000 tryexcept_decorator-0.1.6/tryexcept_decorator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 12:48:46.381332 tryexcept_decorator-0.1.7/
+-rw-rw-rw-   0        0        0     1094 2023-04-07 12:59:02.000000 tryexcept_decorator-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-04-29 12:48:46.381332 tryexcept_decorator-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2023-04-27 15:12:18.000000 tryexcept_decorator-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:48:46.381332 tryexcept_decorator-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-29 12:48:37.000000 tryexcept_decorator-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:48:46.365735 tryexcept_decorator-0.1.7/tryexcept_decorator/
+-rw-rw-rw-   0        0        0       54 2023-04-29 12:48:32.000000 tryexcept_decorator-0.1.7/tryexcept_decorator/__init__.py
+-rw-rw-rw-   0        0        0     4388 2023-04-29 12:17:10.000000 tryexcept_decorator-0.1.7/tryexcept_decorator/decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:48:46.381332 tryexcept_decorator-0.1.7/tryexcept_decorator.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-04-29 12:48:46.000000 tryexcept_decorator-0.1.7/tryexcept_decorator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-29 12:48:46.000000 tryexcept_decorator-0.1.7/tryexcept_decorator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:48:46.000000 tryexcept_decorator-0.1.7/tryexcept_decorator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-29 12:48:46.000000 tryexcept_decorator-0.1.7/tryexcept_decorator.egg-info/top_level.txt
```

### Comparing `tryexcept_decorator-0.1.6/LICENSE` & `tryexcept_decorator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tryexcept_decorator-0.1.6/README.md` & `tryexcept_decorator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tryexcept_decorator-0.1.6/setup.py` & `tryexcept_decorator-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tryexcept_decorator',
     packages=["tryexcept_decorator"],
-    version='0.1.6',
+    version='0.1.7',
     author='Davide Di Grande',
     author_email='davidedigrande.dev@gmail.com',
     description='See README',
     url='https://github.com/davidedigrande/exception_handler_decorator',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
```

### Comparing `tryexcept_decorator-0.1.6/tryexcept_decorator/decorator.py` & `tryexcept_decorator-0.1.7/tryexcept_decorator/decorator.py`

 * *Files identical despite different names*


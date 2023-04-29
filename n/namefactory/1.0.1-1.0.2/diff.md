# Comparing `tmp/namefactory-1.0.1.tar.gz` & `tmp/namefactory-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namefactory-1.0.1.tar", last modified: Sat Apr 29 18:19:23 2023, max compression
+gzip compressed data, was "namefactory-1.0.2.tar", last modified: Sat Apr 29 18:41:03 2023, max compression
```

## Comparing `namefactory-1.0.1.tar` & `namefactory-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 18:19:23.352895 namefactory-1.0.1/
--rw-rw-rw-   0        0        0      243 2023-04-29 18:19:23.351891 namefactory-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-29 16:57:32.000000 namefactory-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 18:19:23.347486 namefactory-1.0.1/namefactory.egg-info/
--rw-rw-rw-   0        0        0      243 2023-04-29 18:19:23.000000 namefactory-1.0.1/namefactory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-29 18:19:23.000000 namefactory-1.0.1/namefactory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:19:23.000000 namefactory-1.0.1/namefactory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 18:19:23.000000 namefactory-1.0.1/namefactory.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:19:23.000000 namefactory-1.0.1/namefactory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 18:19:23.352895 namefactory-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      778 2023-04-29 17:26:56.000000 namefactory-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:41:03.011200 namefactory-1.0.2/
+-rw-rw-rw-   0        0        0      276 2023-04-29 18:41:03.010200 namefactory-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-29 16:57:32.000000 namefactory-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 18:41:02.990170 namefactory-1.0.2/namefactory.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:41:02.000000 namefactory-1.0.2/namefactory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 18:41:03.011200 namefactory-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-04-29 18:36:50.000000 namefactory-1.0.2/setup.py
```

### Comparing `namefactory-1.0.1/README.md` & `namefactory-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `namefactory-1.0.1/setup.py` & `namefactory-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 PACKAGE_NAME = 'namefactory'
 AUTHOR = 'Alan Reynoso Jacuinde'
 AUTHOR_EMAIL = 'alanelhendakari@gmail.com'
 URL = 'https://www.instagram.com/aw.jacuxx/'
 
 LICENSE = 'MIT'
-DESCRIPTION = 'Una librería para hacer cosas geniales'
+DESCRIPTION = 'Una libreria que genera nombres españoles de hombre y mujeres completas'
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
     'pandas'
 ]
 
 setup(
```


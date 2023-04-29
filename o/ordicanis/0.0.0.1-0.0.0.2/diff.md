# Comparing `tmp/ordicanis-0.0.0.1.tar.gz` & `tmp/ordicanis-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ordicanis-0.0.0.1.tar", last modified: Sat Apr 29 12:55:40 2023, max compression
+gzip compressed data, was "dist\ordicanis-0.0.0.2.tar", last modified: Sat Apr 29 13:24:12 2023, max compression
```

## Comparing `ordicanis-0.0.0.1.tar` & `ordicanis-0.0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.602275 ordicanis-0.0.0.1/
--rw-rw-rw-   0        0        0      658 2023-04-29 12:55:40.599279 ordicanis-0.0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.468630 ordicanis-0.0.0.1/jdevtools/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.478613 ordicanis-0.0.0.1/jdevtools/bots/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/bots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.488577 ordicanis-0.0.0.1/jdevtools/data/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.493563 ordicanis-0.0.0.1/jdevtools/extras/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/extras/__init__.py
--rw-rw-rw-   0        0        0      161 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/jCLI.py
--rw-rw-rw-   0        0        0      510 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/jgui.py
--rw-rw-rw-   0        0        0      169 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/jweb.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.514506 ordicanis-0.0.0.1/jdevtools/models/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/models/jkanda.py
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/models/jkissalu.py
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/models/jmesso.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.520491 ordicanis-0.0.0.1/jdevtools/servers/
--rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.1/jdevtools/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:55:40.592298 ordicanis-0.0.0.1/ordicanis.egg-info/
--rw-rw-rw-   0        0        0      658 2023-04-29 12:55:39.000000 ordicanis-0.0.0.1/ordicanis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-29 12:55:40.000000 ordicanis-0.0.0.1/ordicanis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:55:39.000000 ordicanis-0.0.0.1/ordicanis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-29 12:55:39.000000 ordicanis-0.0.0.1/ordicanis.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 12:55:39.000000 ordicanis-0.0.0.1/ordicanis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 12:55:40.604267 ordicanis-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2070 2023-04-29 12:55:08.000000 ordicanis-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.481803 ordicanis-0.0.0.2/
+-rw-rw-rw-   0        0        0      818 2023-04-29 13:24:12.479813 ordicanis-0.0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.403015 ordicanis-0.0.0.2/jdevtools/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.405008 ordicanis-0.0.0.2/jdevtools/bots/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/bots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.409024 ordicanis-0.0.0.2/jdevtools/data/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.411993 ordicanis-0.0.0.2/jdevtools/extras/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/extras/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/jCLI.py
+-rw-rw-rw-   0        0        0      510 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/jgui.py
+-rw-rw-rw-   0        0        0      169 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/jweb.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.429941 ordicanis-0.0.0.2/jdevtools/models/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/models/jkanda.py
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/models/jkissalu.py
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/models/jmesso.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.432933 ordicanis-0.0.0.2/jdevtools/servers/
+-rw-rw-rw-   0        0        0        0 2023-03-02 14:48:24.000000 ordicanis-0.0.0.2/jdevtools/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:24:12.473825 ordicanis-0.0.0.2/ordicanis.egg-info/
+-rw-rw-rw-   0        0        0      818 2023-04-29 13:24:12.000000 ordicanis-0.0.0.2/ordicanis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-29 13:24:12.000000 ordicanis-0.0.0.2/ordicanis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:24:12.000000 ordicanis-0.0.0.2/ordicanis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-29 13:24:12.000000 ordicanis-0.0.0.2/ordicanis.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 13:24:12.000000 ordicanis-0.0.0.2/ordicanis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:24:12.483799 ordicanis-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2023-04-29 13:24:03.000000 ordicanis-0.0.0.2/setup.py
```

### Comparing `ordicanis-0.0.0.1/setup.py` & `ordicanis-0.0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 import atexit
 
 setup(
     # name=['ordicanis', 'ordicanis'],#name='ordicanis',
     name='ordicanis',
-    version='0.0.0.1',
+    version='0.0.0.2',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'ordicanis = ordicanis.__main__:main'
         ]
     },
     author='Juste Elysée MALNADILA',
     author_email='malandilajusteelysee@gmail.com',
-    # description=''' 👨‍💻"ordicanis" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛''',
+    description='''💎👨‍💻"ordicanis" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛''',
     # long_description=''' this is a Python package designed to facilitate the importation of missing modules during coding. Rather than requiring manual importation of modules that have not been previously utilized, "ordicanis" enables automatic detection and importation of such modules in real-time. This feature streamlines the coding process by eliminating the need for users to manually manage imports, allowing them to focus on writing code without distraction. "ordicanis" is available for installation via PyPI using pip.''',
     url='https://github.com/yourusername/ordicanis',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         # 'Programming Language :: Python :: 3.6',
```


# Comparing `tmp/mrdoxmrgt-0.1.4.tar.gz` & `tmp/mrdoxmrgt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.1.4.tar", last modified: Sat Apr 29 09:45:14 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.1.5.tar", last modified: Sat Apr 29 09:53:14 2023, max compression
```

## Comparing `mrdoxmrgt-0.1.4.tar` & `mrdoxmrgt-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      800 2023-04-29 09:45:16.000000 mrdoxmrgt-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-14 09:24:50.000000 mrdoxmrgt-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      800 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 09:45:14.000000 mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 09:45:16.000000 mrdoxmrgt-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-04-29 09:44:32.000000 mrdoxmrgt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-28 13:12:16.000000 mrdoxmrgt-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-04-29 09:53:16.000000 mrdoxmrgt-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-28 13:12:16.000000 mrdoxmrgt-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:12:16.000000 mrdoxmrgt-0.1.5/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     3792 2023-04-28 13:12:16.000000 mrdoxmrgt-0.1.5/mrdoxmrgt/main.py
+-rw-rw-rw-   0        0        0    15122 2023-04-28 13:12:16.000000 mrdoxmrgt-0.1.5/mrdoxmrgt/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 09:53:14.000000 mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 09:53:16.000000 mrdoxmrgt-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-04-29 09:52:46.000000 mrdoxmrgt-0.1.5/setup.py
```

### Comparing `mrdoxmrgt-0.1.4/LICENSE` & `mrdoxmrgt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.1.4/PKG-INFO` & `mrdoxmrgt-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.1.4/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.1.5/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/gtf
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.1.4/setup.py` & `mrdoxmrgt-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.1.4",
+    version="0.1.5",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/gtf',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
@@ -19,15 +19,15 @@
             'Intended Audience :: Developers',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
             'Programming Language :: Python :: 3',
             'Operating System :: OS Independent',
             'Environment :: Console',
     ],
-    install_requires=["requests", "random2"],
+    install_requires=["requests", "random2", "zipfile"],
     license='GPL',
     entry_points={
             'console_scripts': [
                 'mrdoxmrgt = mrdoxmrgt.main:Main',
             ],
     },
     python_requires='>=3.5'
```


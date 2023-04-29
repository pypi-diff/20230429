# Comparing `tmp/selfetch-0.0.0.0.tar.gz` & `tmp/selfetch-0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selfetch-0.0.0.0.tar", last modified: Sat Apr 29 12:00:52 2023, max compression
+gzip compressed data, was "dist\selfetch-0.0.0.1.tar", last modified: Sat Apr 29 13:33:11 2023, max compression
```

## Comparing `selfetch-0.0.0.0.tar` & `selfetch-0.0.0.1.tar`

### file list

```diff
@@ -1,10 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:00:52.751819 selfetch-0.0.0.0/
--rw-rw-rw-   0        0        0     1318 2023-04-29 12:00:52.748804 selfetch-0.0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:00:52.744812 selfetch-0.0.0.0/selfetch.egg-info/
--rw-rw-rw-   0        0        0     1318 2023-04-29 12:00:52.000000 selfetch-0.0.0.0/selfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-04-29 12:00:52.000000 selfetch-0.0.0.0/selfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:00:52.000000 selfetch-0.0.0.0/selfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-29 12:00:52.000000 selfetch-0.0.0.0/selfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:00:52.000000 selfetch-0.0.0.0/selfetch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 12:00:52.752792 selfetch-0.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2055 2023-04-29 12:00:48.000000 selfetch-0.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.614780 selfetch-0.0.0.1/
+-rw-rw-rw-   0        0        0     1317 2023-04-29 13:33:11.608367 selfetch-0.0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.497759 selfetch-0.0.0.1/jdevtools/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.508703 selfetch-0.0.0.1/jdevtools/bots/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/bots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.512689 selfetch-0.0.0.1/jdevtools/data/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.515671 selfetch-0.0.0.1/jdevtools/extras/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/extras/__init__.py
+-rw-rw-rw-   0        0        0       94 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/jCLI.py
+-rw-rw-rw-   0        0        0      467 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/jgui.py
+-rw-rw-rw-   0        0        0       57 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/jweb.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.523649 selfetch-0.0.0.1/jdevtools/models/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/models/jkanda.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/models/jkissalu.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/models/jmesso.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.532629 selfetch-0.0.0.1/jdevtools/servers/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:21:36.000000 selfetch-0.0.0.1/jdevtools/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:11.600547 selfetch-0.0.0.1/selfetch.egg-info/
+-rw-rw-rw-   0        0        0     1317 2023-04-29 13:33:11.000000 selfetch-0.0.0.1/selfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-29 13:33:11.000000 selfetch-0.0.0.1/selfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:33:11.000000 selfetch-0.0.0.1/selfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-29 13:33:11.000000 selfetch-0.0.0.1/selfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 13:33:11.000000 selfetch-0.0.0.1/selfetch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:33:11.615929 selfetch-0.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2054 2023-04-29 13:32:52.000000 selfetch-0.0.0.1/setup.py
```

### Comparing `selfetch-0.0.0.0/PKG-INFO` & `selfetch-0.0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: selfetch
-Version: 0.0.0.0
-Summary:  👨‍💻"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
+Version: 0.0.0.1
+Summary:  💦♻️"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
 Home-page: https://github.com/yourusername/selfetch
 Author: Juste Elysée MALNADILA
 Author-email: malandilajusteelysee@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selfetch-0.0.0.0/selfetch.egg-info/PKG-INFO` & `selfetch-0.0.0.1/selfetch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: selfetch
-Version: 0.0.0.0
-Summary:  👨‍💻"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
+Version: 0.0.0.1
+Summary:  💦♻️"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛
 Home-page: https://github.com/yourusername/selfetch
 Author: Juste Elysée MALNADILA
 Author-email: malandilajusteelysee@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `selfetch-0.0.0.0/setup.py` & `selfetch-0.0.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 import atexit
 
 setup(
     # name=['selfetch', 'Selfetch'],#name='selfetch',
     name='selfetch',
-    version='0.0.0.0',
+    version='0.0.0.1',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'selfetch = selfetch.__main__:main'
         ]
     },
     author='Juste Elysée MALNADILA',
     author_email='malandilajusteelysee@gmail.com',
-    description=''' 👨‍💻"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛''',
+    description=''' 💦♻️"selfetch" is a Python package that automatically imports missing modules on-the-fly, saving time and effort during coding 🛠️⌛''',
     long_description=''' this is a Python package designed to facilitate the importation of missing modules during coding. Rather than requiring manual importation of modules that have not been previously utilized, "selfetch" enables automatic detection and importation of such modules in real-time. This feature streamlines the coding process by eliminating the need for users to manually manage imports, allowing them to focus on writing code without distraction. "selfetch" is available for installation via PyPI using pip.''',
     url='https://github.com/yourusername/selfetch',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         # 'Programming Language :: Python :: 3.6',
```


# Comparing `tmp/flet-web-template-0.1.2.tar.gz` & `tmp/flet-web-template-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-web-template-0.1.2.tar", last modified: Sat Apr 29 15:56:05 2023, max compression
+gzip compressed data, was "flet-web-template-0.1.3.tar", last modified: Sat Apr 29 16:05:01 2023, max compression
```

## Comparing `flet-web-template-0.1.2.tar` & `flet-web-template-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:56:05.153653 flet-web-template-0.1.2/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.2/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:56:05.153470 flet-web-template-0.1.2/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.2/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:56:05.149816 flet-web-template-0.1.2/command/
--rw-r--r--   0 ahmad      (501) staff       (20)     9226 2023-04-29 15:48:41.000000 flet-web-template-0.1.2/command/cli.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:56:05.151622 flet-web-template-0.1.2/flet_template/
--rw-r--r--   0 ahmad      (501) staff       (20)      178 2023-04-29 14:22:03.000000 flet-web-template-0.1.2/flet_template/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.2/flet_template/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.2/flet_template/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.2/flet_template/route_base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.2/flet_template/script.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:56:05.153083 flet-web-template-0.1.2/flet_web_template.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       71 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       41 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 15:56:05.000000 flet-web-template-0.1.2/flet_web_template.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 15:56:05.153705 flet-web-template-0.1.2/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      812 2023-04-29 15:55:53.000000 flet-web-template-0.1.2/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:56:05.153245 flet-web-template-0.1.2/test/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.2/test/test.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:05:01.527469 flet-web-template-0.1.3/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.3/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:05:01.527271 flet-web-template-0.1.3/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.3/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:05:01.523762 flet-web-template-0.1.3/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)     9226 2023-04-29 15:48:41.000000 flet-web-template-0.1.3/command/cli.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:05:01.525522 flet-web-template-0.1.3/flet_template/
+-rw-r--r--   0 ahmad      (501) staff       (20)      178 2023-04-29 14:22:03.000000 flet-web-template-0.1.3/flet_template/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.3/flet_template/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.3/flet_template/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.3/flet_template/route_base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.3/flet_template/script.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:05:01.526874 flet-web-template-0.1.3/flet_web_template.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       57 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       41 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 16:05:01.000000 flet-web-template-0.1.3/flet_web_template.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 16:05:01.527535 flet-web-template-0.1.3/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      798 2023-04-29 16:04:45.000000 flet-web-template-0.1.3/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:05:01.527046 flet-web-template-0.1.3/test/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.3/test/test.py
```

### Comparing `flet-web-template-0.1.2/LICENSE` & `flet-web-template-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.2/PKG-INFO` & `flet-web-template-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.2
+Version: 0.1.3
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.2/command/cli.py` & `flet-web-template-0.1.3/command/cli.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.2/flet_template/base.py` & `flet-web-template-0.1.3/flet_template/base.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.2/flet_template/script.py` & `flet-web-template-0.1.3/flet_template/script.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.2/flet_web_template.egg-info/PKG-INFO` & `flet-web-template-0.1.3/flet_web_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.2
+Version: 0.1.3
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.2/setup.py` & `flet-web-template-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name="flet-web-template",
-    version="0.1.2",
+    version="0.1.3",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/flet_boilerplate",
     packages=["flet_template", "command"],
     install_requires=["click==8.1.3", "flet==0.5.2", " pickle5==0.0.11"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
-        "console_scripts": ["flet_material_init=flet_template.command.cli:init"],
+        "console_scripts": ["flet_material_init=command.cli:init"],
     },
     keywords=["python web templates", "web application", "development"],
 )
```


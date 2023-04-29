# Comparing `tmp/flet-web-template-0.1.5.tar.gz` & `tmp/flet-web-template-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-web-template-0.1.5.tar", last modified: Sat Apr 29 16:16:01 2023, max compression
+gzip compressed data, was "flet-web-template-0.1.6.tar", last modified: Sat Apr 29 16:22:54 2023, max compression
```

## Comparing `flet-web-template-0.1.5.tar` & `flet-web-template-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:16:01.424309 flet-web-template-0.1.5/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.5/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:16:01.424128 flet-web-template-0.1.5/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.5/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:16:01.420966 flet-web-template-0.1.5/command/
--rw-r--r--   0 ahmad      (501) staff       (20)     9245 2023-04-29 16:15:45.000000 flet-web-template-0.1.5/command/cli.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:16:01.422445 flet-web-template-0.1.5/flet_template/
--rw-r--r--   0 ahmad      (501) staff       (20)      186 2023-04-29 16:11:11.000000 flet-web-template-0.1.5/flet_template/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.5/flet_template/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.5/flet_template/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.5/flet_template/route_base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.5/flet_template/script.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:16:01.423714 flet-web-template-0.1.5/flet_web_template.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       57 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       41 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 16:16:01.000000 flet-web-template-0.1.5/flet_web_template.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 16:16:01.424366 flet-web-template-0.1.5/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      798 2023-04-29 16:15:50.000000 flet-web-template-0.1.5/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:16:01.423897 flet-web-template-0.1.5/test/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.5/test/test.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.304240 flet-web-template-0.1.6/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.6/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:22:54.303903 flet-web-template-0.1.6/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.6/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.301182 flet-web-template-0.1.6/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)     9245 2023-04-29 16:15:45.000000 flet-web-template-0.1.6/command/cli.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.302564 flet-web-template-0.1.6/flet_template/
+-rw-r--r--   0 ahmad      (501) staff       (20)      186 2023-04-29 16:11:11.000000 flet-web-template-0.1.6/flet_template/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.6/flet_template/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.6/flet_template/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.6/flet_template/route_base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.6/flet_template/script.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.303571 flet-web-template-0.1.6/flet_web_template.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       57 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       53 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 16:22:54.304287 flet-web-template-0.1.6/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      813 2023-04-29 16:22:20.000000 flet-web-template-0.1.6/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.303704 flet-web-template-0.1.6/test/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.6/test/test.py
```

### Comparing `flet-web-template-0.1.5/LICENSE` & `flet-web-template-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.5/PKG-INFO` & `flet-web-template-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.5/command/cli.py` & `flet-web-template-0.1.6/command/cli.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.5/flet_template/base.py` & `flet-web-template-0.1.6/flet_template/base.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.5/flet_template/script.py` & `flet-web-template-0.1.6/flet_template/script.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.5/flet_web_template.egg-info/PKG-INFO` & `flet-web-template-0.1.6/flet_web_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.5/setup.py` & `flet-web-template-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="flet-web-template",
-    version="0.1.5",
+    version="0.1.6",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/flet_boilerplate",
     packages=["flet_template", "command"],
-    install_requires=["click==8.1.3", "flet==0.5.2", " pickle5==0.0.11"],
+    install_requires=["click==8.1.3", "flet==0.5.2", " pickle5==0.0.11", "PyYAML==6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["flet_material_init=command.cli:init"],
```


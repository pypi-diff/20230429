# Comparing `tmp/flet-web-template-0.1.6.tar.gz` & `tmp/flet-web-template-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-web-template-0.1.6.tar", last modified: Sat Apr 29 16:22:54 2023, max compression
+gzip compressed data, was "flet-web-template-0.1.7.tar", last modified: Sat Apr 29 16:31:29 2023, max compression
```

## Comparing `flet-web-template-0.1.6.tar` & `flet-web-template-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.304240 flet-web-template-0.1.6/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.6/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:22:54.303903 flet-web-template-0.1.6/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.6/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.301182 flet-web-template-0.1.6/command/
--rw-r--r--   0 ahmad      (501) staff       (20)     9245 2023-04-29 16:15:45.000000 flet-web-template-0.1.6/command/cli.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.302564 flet-web-template-0.1.6/flet_template/
--rw-r--r--   0 ahmad      (501) staff       (20)      186 2023-04-29 16:11:11.000000 flet-web-template-0.1.6/flet_template/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.6/flet_template/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.6/flet_template/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.6/flet_template/route_base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.6/flet_template/script.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.303571 flet-web-template-0.1.6/flet_web_template.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       57 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       53 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 16:22:54.000000 flet-web-template-0.1.6/flet_web_template.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 16:22:54.304287 flet-web-template-0.1.6/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      813 2023-04-29 16:22:20.000000 flet-web-template-0.1.6/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:22:54.303704 flet-web-template-0.1.6/test/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.6/test/test.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:31:29.671245 flet-web-template-0.1.7/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.7/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:31:29.671107 flet-web-template-0.1.7/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.7/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:31:29.668684 flet-web-template-0.1.7/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)     9273 2023-04-29 16:30:39.000000 flet-web-template-0.1.7/command/cli.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:31:29.669871 flet-web-template-0.1.7/flet_template/
+-rw-r--r--   0 ahmad      (501) staff       (20)      186 2023-04-29 16:11:11.000000 flet-web-template-0.1.7/flet_template/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.7/flet_template/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.7/flet_template/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.7/flet_template/route_base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.7/flet_template/script.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:31:29.670820 flet-web-template-0.1.7/flet_web_template.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       57 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       53 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 16:31:29.000000 flet-web-template-0.1.7/flet_web_template.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 16:31:29.671290 flet-web-template-0.1.7/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      813 2023-04-29 16:31:14.000000 flet-web-template-0.1.7/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 16:31:29.670944 flet-web-template-0.1.7/test/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.7/test/test.py
```

### Comparing `flet-web-template-0.1.6/LICENSE` & `flet-web-template-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.6/PKG-INFO` & `flet-web-template-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.6
+Version: 0.1.7
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.6/command/cli.py` & `flet-web-template-0.1.7/command/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,32 +234,32 @@
     nav:
     - Home: "index.py"
     - Page: "page.py"
     """
         )
 
     # Create templates directory if it doesn't exist
-    if not os.path.exists("templates"):
-        os.makedirs("templates")
+    if not os.path.exists("flet_template"):
+        os.makedirs("flet_template")
 
     # Define the list of files to be generated
     file_list = ["__init__.py", "main.py", "base.py", "route_base.py", "script.py"]
 
     # Generate each file in the templates directory
     for file_name in file_list:
-        file_path = os.path.join("templates", file_name)
+        file_path = os.path.join("flet_template", file_name)
         open(file_path, "a").close()
 
         # If it's the __init__.py file, write the import statements
         if file_name == "__init__.py":
             with open(file_path, "w") as f:
-                f.write("from templates.base import base_page\n")
-                f.write("from templates.main import main\n")
-                f.write("from templates.script import run_template_script\n")
-                f.write("from templates.route_base import route_page\n")
+                f.write("from flet_template.base import base_page\n")
+                f.write("from flet_template.main import main\n")
+                f.write("from flet_template.script import run_template_script\n")
+                f.write("from flet_template.route_base import route_page\n")
 
         # If it's the main.py file, write the main statements
         if file_name == "main.py":
             with open(file_path, "w") as f:
                 f.write(main_thread)
 
         # If it's the base.py file, write the main statements
```

### Comparing `flet-web-template-0.1.6/flet_template/base.py` & `flet-web-template-0.1.7/flet_template/base.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.6/flet_template/script.py` & `flet-web-template-0.1.7/flet_template/script.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.6/flet_web_template.egg-info/PKG-INFO` & `flet-web-template-0.1.7/flet_web_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.6
+Version: 0.1.7
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.6/setup.py` & `flet-web-template-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="flet-web-template",
-    version="0.1.6",
+    version="0.1.7",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/flet_boilerplate",
     packages=["flet_template", "command"],
```


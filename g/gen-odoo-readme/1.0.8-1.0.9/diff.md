# Comparing `tmp/gen-odoo-readme-1.0.8.tar.gz` & `tmp/gen-odoo-readme-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-odoo-readme-1.0.8.tar", last modified: Sat Apr 22 17:29:49 2023, max compression
+gzip compressed data, was "gen-odoo-readme-1.0.9.tar", last modified: Thu Apr 27 01:26:35 2023, max compression
```

## Comparing `gen-odoo-readme-1.0.8.tar` & `gen-odoo-readme-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 17:29:49.000000 gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:49.815744 gen-odoo-readme-1.0.8/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/gen_addon_readme.template
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/gen_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-22 17:29:36.000000 gen-odoo-readme-1.0.8/tools/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:26:35.051637 gen-odoo-readme-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-27 01:26:35.051637 gen-odoo-readme-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:26:35.051637 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 01:26:35.000000 gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 01:26:35.051637 gen-odoo-readme-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:26:35.051637 gen-odoo-readme-1.0.9/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/tools/gen_addon_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/tools/gen_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-27 01:26:19.000000 gen-odoo-readme-1.0.9/tools/manifest.py
```

### Comparing `gen-odoo-readme-1.0.8/LICENSE` & `gen-odoo-readme-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-1.0.8/PKG-INFO` & `gen-odoo-readme-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-1.0.8/README.md` & `gen-odoo-readme-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-1.0.8/gen_odoo_readme.egg-info/PKG-INFO` & `gen-odoo-readme-1.0.9/gen_odoo_readme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-odoo-readme
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool to create README.rst files for Odoo
 Home-page: https://github.com/jobiols/gen-readme
 Author: Jorge E. Obiols
 Author-email: jorge.obiols@gmail.com
 Keywords: odoo documentation readme rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gen-odoo-readme-1.0.8/setup.py` & `gen-odoo-readme-1.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
-from tools import __version__
-
 setuptools.setup(
     name="gen-odoo-readme",
-    version=__version__,
     author="Jorge E. Obiols",
     description="Tool to create README.rst files for Odoo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jobiols/gen-readme",
     author_email="jorge.obiols@gmail.com",
     python_requires=">=3.8",
```

### Comparing `gen-odoo-readme-1.0.8/tools/gen_addon_readme.template` & `gen-odoo-readme-1.0.9/tools/gen_addon_readme.template`

 * *Files identical despite different names*

### Comparing `gen-odoo-readme-1.0.8/tools/gen_readme.py` & `gen-odoo-readme-1.0.9/tools/gen_readme.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,14 +224,19 @@
         # Agregar una linea en blanco al final del RST para que no falle el test
         # W7908(missing-newline-extrafiles).
         rf.write("\n")
     return readme_filename
 
 
 @click.command()
+@click.argument(
+    "files",
+    type=click.Path(exists=False),
+    nargs=-1,
+)
 @click.option(
     "--org-name",
     required=True,
     help="Organization name",
 )
 @click.option(
     "--repo-name",
@@ -241,29 +246,31 @@
 @click.option(
     "--branch",
     required=True,
     help="Odoo series. eg 11.0.",
 )
 @click.option(
     "--addons-dir",
-    type=click.Path(dir_okay=True, file_okay=False, exists=True),
+    type=click.Path(dir_okay=True, file_okay=False, exists=False),
     required=False,
     help="Directory containing several addons, the README will be "
-    "generated for all installable addons found there.",
+    "generated for all installable addons found there...",
 )
 @click.option(
     "--gen-html/--no-gen-html",
     default=True,
     help="Generate index html file.",
 )
-def gen_readme(org_name, repo_name, branch, addons_dir, gen_html):
+def gen_readme(files, org_name, repo_name, branch, addons_dir, gen_html):
     """main function"""
 
-    print("Gen Readme ------------------")
-    print(os.path.abspath(__file__))
+    print("Gen Readme!")
+    print("path -->", os.path.abspath(__file__))
+    print("files -- ", files)
+    exit()
 
     addons = list()
     if addons_dir:
         addons.extend(find_addons(addons_dir))
     readme_filenames = []
     for addon_name, addon_dir, manifest in addons:
         if not os.path.exists(
@@ -277,11 +284,7 @@
         readme_filenames.append(readme_filename)
         if gen_html:
             if not manifest.get("preloadable", True):
                 continue
             index_filename = gen_one_addon_index(readme_filename)
             if index_filename:
                 readme_filenames.append(index_filename)
-
-
-if __name__ == "__main__":
-    gen_readme()
```

### Comparing `gen-odoo-readme-1.0.8/tools/manifest.py` & `gen-odoo-readme-1.0.9/tools/manifest.py`

 * *Files identical despite different names*


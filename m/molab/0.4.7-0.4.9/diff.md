# Comparing `tmp/molab-0.4.7.tar.gz` & `tmp/molab-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molab-0.4.7.tar", last modified: Fri Apr 28 22:52:09 2023, max compression
+gzip compressed data, was "molab-0.4.9.tar", last modified: Sat Apr 29 03:19:32 2023, max compression
```

## Comparing `molab-0.4.7.tar` & `molab-0.4.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 22:52:09.548351 molab-0.4.7/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 22:52:09.547351 molab-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-28 22:51:53.000000 molab-0.4.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 22:52:09.542351 molab-0.4.7/molab/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-28 22:51:53.000000 molab-0.4.7/molab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-28 22:51:53.000000 molab-0.4.7/molab/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-28 22:51:53.000000 molab-0.4.7/molab/courses.py
--rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-28 22:51:53.000000 molab-0.4.7/molab/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-28 22:51:53.000000 molab-0.4.7/molab/destroy.py
--rw-rw-rw-   0 root         (0) root         (0)    20308 2023-04-28 22:51:53.000000 molab-0.4.7/molab/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 22:52:09.547351 molab-0.4.7/molab/template_files/
--rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/MorpheusImage.png
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/admin_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/automation_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/git_auth_type_pat.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/install_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/instance_provisioning_payload.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/manual_option_list_aws_regions.json
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/platform_setup.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 22:51:53.000000 molab-0.4.7/molab/template_files/troubleshooting_class_config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 22:52:09.544351 molab-0.4.7/molab.egg-info/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 22:52:09.000000 molab-0.4.7/molab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-28 22:52:09.000000 molab-0.4.7/molab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 22:52:09.000000 molab-0.4.7/molab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-28 22:52:09.000000 molab-0.4.7/molab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 22:52:09.000000 molab-0.4.7/molab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 22:52:09.548351 molab-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-28 22:51:53.000000 molab-0.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 03:19:32.772611 molab-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-29 03:19:32.771694 molab-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-29 03:19:16.000000 molab-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 03:19:32.766194 molab-0.4.9/molab/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-29 03:19:16.000000 molab-0.4.9/molab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-29 03:19:16.000000 molab-0.4.9/molab/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-29 03:19:16.000000 molab-0.4.9/molab/courses.py
+-rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-29 03:19:16.000000 molab-0.4.9/molab/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-29 03:19:16.000000 molab-0.4.9/molab/destroy.py
+-rw-rw-rw-   0 root         (0) root         (0)    20308 2023-04-29 03:19:16.000000 molab-0.4.9/molab/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 03:19:32.771694 molab-0.4.9/molab/template_files/
+-rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/MorpheusImage.png
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/admin_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/automation_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/git_auth_type_pat.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/install_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/instance_provisioning_payload.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/manual_option_list_aws_regions.json
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/platform_setup.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-29 03:19:16.000000 molab-0.4.9/molab/template_files/troubleshooting_class_config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 03:19:32.768027 molab-0.4.9/molab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-29 03:19:32.000000 molab-0.4.9/molab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-29 03:19:32.000000 molab-0.4.9/molab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 03:19:32.000000 molab-0.4.9/molab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-29 03:19:32.000000 molab-0.4.9/molab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-29 03:19:32.000000 molab-0.4.9/molab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 03:19:32.772611 molab-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-29 03:19:16.000000 molab-0.4.9/setup.py
```

### Comparing `molab-0.4.7/PKG-INFO` & `molab-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.7
+Version: 0.4.9
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.7/molab/configure.py` & `molab-0.4.9/molab/configure.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/courses.py` & `molab-0.4.9/molab/courses.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/deploy.py` & `molab-0.4.9/molab/deploy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/destroy.py` & `molab-0.4.9/molab/destroy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/helpers.py` & `molab-0.4.9/molab/helpers.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/MorpheusImage.png` & `molab-0.4.9/molab/template_files/MorpheusImage.png`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/admin_class_config.json` & `molab-0.4.9/molab/template_files/admin_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/automation_class_config.json` & `molab-0.4.9/molab/template_files/automation_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/install_class_config.json` & `molab-0.4.9/molab/template_files/install_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/instance_provisioning_payload.json` & `molab-0.4.9/molab/template_files/instance_provisioning_payload.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/manual_option_list_aws_regions.json` & `molab-0.4.9/molab/template_files/manual_option_list_aws_regions.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab/template_files/troubleshooting_class_config.json` & `molab-0.4.9/molab/template_files/troubleshooting_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/molab.egg-info/PKG-INFO` & `molab-0.4.9/molab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.7
+Version: 0.4.9
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.7/molab.egg-info/SOURCES.txt` & `molab-0.4.9/molab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molab-0.4.7/setup.py` & `molab-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     author="Sean Jabro",
     author_email="sean.jabro@outlook.com",
     name='molab',
     license="MIT",
     description='molab is a python package for configuring Morpheus training lab environments.',
-    version='0.4.7',
+    version='0.4.9',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/morpheus_training/molab',
     packages=find_packages() + find_packages(where='template_files'),
     package_dir={'template_files': 'template_files'},
     package_data={'molab': ['template_files/*.*']},
     python_requires=">=3.8",
```


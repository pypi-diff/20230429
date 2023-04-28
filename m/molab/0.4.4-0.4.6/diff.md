# Comparing `tmp/molab-0.4.4.tar.gz` & `tmp/molab-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molab-0.4.4.tar", last modified: Fri Apr 28 20:05:13 2023, max compression
+gzip compressed data, was "molab-0.4.6.tar", last modified: Fri Apr 28 21:27:37 2023, max compression
```

## Comparing `molab-0.4.4.tar` & `molab-0.4.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:05:13.904782 molab-0.4.4/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 20:05:13.904782 molab-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-28 20:04:57.000000 molab-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:05:13.900198 molab-0.4.4/molab/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-28 20:04:57.000000 molab-0.4.4/molab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-28 20:04:57.000000 molab-0.4.4/molab/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-28 20:04:57.000000 molab-0.4.4/molab/courses.py
--rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-28 20:04:57.000000 molab-0.4.4/molab/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-28 20:04:57.000000 molab-0.4.4/molab/destroy.py
--rw-rw-rw-   0 root         (0) root         (0)    20151 2023-04-28 20:04:57.000000 molab-0.4.4/molab/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:05:13.904782 molab-0.4.4/molab/template_files/
--rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/MorpheusImage.png
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/admin_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/automation_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/git_auth_type_pat.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/install_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/instance_provisioning_payload.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/manual_option_list_aws_regions.json
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/platform_setup.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 20:04:57.000000 molab-0.4.4/molab/template_files/troubleshooting_class_config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:05:13.901115 molab-0.4.4/molab.egg-info/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 20:05:13.000000 molab-0.4.4/molab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-28 20:05:13.000000 molab-0.4.4/molab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:05:13.000000 molab-0.4.4/molab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-28 20:05:13.000000 molab-0.4.4/molab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 20:05:13.000000 molab-0.4.4/molab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 20:05:13.904782 molab-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-28 20:04:57.000000 molab-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:27:37.323678 molab-0.4.6/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 21:27:37.323678 molab-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-28 21:27:20.000000 molab-0.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:27:37.317678 molab-0.4.6/molab/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-28 21:27:20.000000 molab-0.4.6/molab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-28 21:27:20.000000 molab-0.4.6/molab/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-28 21:27:20.000000 molab-0.4.6/molab/courses.py
+-rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-28 21:27:20.000000 molab-0.4.6/molab/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-28 21:27:20.000000 molab-0.4.6/molab/destroy.py
+-rw-rw-rw-   0 root         (0) root         (0)    20193 2023-04-28 21:27:20.000000 molab-0.4.6/molab/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:27:37.323678 molab-0.4.6/molab/template_files/
+-rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/MorpheusImage.png
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/admin_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/automation_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/git_auth_type_pat.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/install_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/instance_provisioning_payload.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/manual_option_list_aws_regions.json
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/platform_setup.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-28 21:27:20.000000 molab-0.4.6/molab/template_files/troubleshooting_class_config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:27:37.319678 molab-0.4.6/molab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-28 21:27:37.000000 molab-0.4.6/molab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-28 21:27:37.000000 molab-0.4.6/molab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:27:37.000000 molab-0.4.6/molab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-28 21:27:37.000000 molab-0.4.6/molab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 21:27:37.000000 molab-0.4.6/molab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 21:27:37.323678 molab-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-28 21:27:20.000000 molab-0.4.6/setup.py
```

### Comparing `molab-0.4.4/PKG-INFO` & `molab-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.4
+Version: 0.4.6
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.4/molab/configure.py` & `molab-0.4.6/molab/configure.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/courses.py` & `molab-0.4.6/molab/courses.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/deploy.py` & `molab-0.4.6/molab/deploy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/destroy.py` & `molab-0.4.6/molab/destroy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/helpers.py` & `molab-0.4.6/molab/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,25 +341,26 @@
         "executeTarget": "local",
         "retryable": False,
         "allowCustomConfig": False
       }
     }
     body = json.dumps(jbody)
     try:
-        resp = requests.post(f'{url}{endpoint}', headers=headers, data=body, verify=False)
+        resp = requests.post(f'https://{url}{endpoint}', headers=headers, data=body, verify=False)
     except Exception as e:
         logger.error(e)
         return
     if "200" in str(resp):
         data = resp.json()
         logger.info(f'Successfully created {resource_type} {name} at ID: {data[resource_type]["id"]}')
         logger.info(f'Returning {resource_type} ID')
         return data[resource_type]["id"]
     else:
         logger.error(f'API call failed with response: {resp}')
+        logger.error(resp.json())
         exit(0)
 
 def _get_workflow_id_by_name(url,headers,name):
     logger.info(f'Begin attempt to get workflow by name')
     endpoint = "/api/task-sets"
     resource_type = "taskSets"
     try:
```

### Comparing `molab-0.4.4/molab/template_files/MorpheusImage.png` & `molab-0.4.6/molab/template_files/MorpheusImage.png`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/admin_class_config.json` & `molab-0.4.6/molab/template_files/admin_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/automation_class_config.json` & `molab-0.4.6/molab/template_files/automation_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/install_class_config.json` & `molab-0.4.6/molab/template_files/install_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/instance_provisioning_payload.json` & `molab-0.4.6/molab/template_files/instance_provisioning_payload.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/manual_option_list_aws_regions.json` & `molab-0.4.6/molab/template_files/manual_option_list_aws_regions.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab/template_files/troubleshooting_class_config.json` & `molab-0.4.6/molab/template_files/troubleshooting_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/molab.egg-info/PKG-INFO` & `molab-0.4.6/molab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.4
+Version: 0.4.6
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.4/molab.egg-info/SOURCES.txt` & `molab-0.4.6/molab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molab-0.4.4/setup.py` & `molab-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     author="Sean Jabro",
     author_email="sean.jabro@outlook.com",
     name='molab',
     license="MIT",
     description='molab is a python package for configuring Morpheus training lab environments.',
-    version='0.4.4',
+    version='0.4.6',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/morpheus_training/molab',
     packages=find_packages() + find_packages(where='template_files'),
     package_dir={'template_files': 'template_files'},
     package_data={'molab': ['template_files/*.*']},
     python_requires=">=3.8",
```


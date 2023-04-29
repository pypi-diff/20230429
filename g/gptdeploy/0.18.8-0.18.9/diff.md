# Comparing `tmp/gptdeploy-0.18.8.tar.gz` & `tmp/gptdeploy-0.18.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.18.8.tar", last modified: Mon Apr 10 20:22:12 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.9.tar", last modified: Mon Apr 10 20:30:58 2023, max compression
```

## Comparing `gptdeploy-0.18.8.tar` & `gptdeploy-0.18.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/gptdeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/executor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/key_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:22:12.000000 gptdeploy-0.18.8/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 20:21:57.000000 gptdeploy-0.18.8/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/gptdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/executor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:30:58.000000 gptdeploy-0.18.9/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 20:30:36.000000 gptdeploy-0.18.9/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.18.8/PKG-INFO` & `gptdeploy-0.18.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.8
+Version: 0.18.9
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.8 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.9 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.8/README.md` & `gptdeploy-0.18.9/README.md`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.9/gptdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.8
+Version: 0.18.9
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.8 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.9 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.18.8/setup.py` & `gptdeploy-0.18.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.18.8',
+    version='0.18.9',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
```

### Comparing `gptdeploy-0.18.8/src/cli.py` & `gptdeploy-0.18.9/src/cli.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/constants.py` & `gptdeploy-0.18.9/src/constants.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/executor_factory.py` & `gptdeploy-0.18.9/src/executor_factory.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/gpt.py` & `gptdeploy-0.18.9/src/gpt.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/jina_cloud.py` & `gptdeploy-0.18.9/src/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/key_handling.py` & `gptdeploy-0.18.9/src/key_handling.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/prompt_system.py` & `gptdeploy-0.18.9/src/prompt_system.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/prompt_tasks.py` & `gptdeploy-0.18.9/src/prompt_tasks.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/server.py` & `gptdeploy-0.18.9/src/server.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/utils/io.py` & `gptdeploy-0.18.9/src/utils/io.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.8/src/utils/string_tools.py` & `gptdeploy-0.18.9/src/utils/string_tools.py`

 * *Files identical despite different names*


# Comparing `tmp/clueai-0.0.2.2.5.tar.gz` & `tmp/clueai-0.0.2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clueai-0.0.2.2.5.tar", last modified: Sat Apr 29 06:34:49 2023, max compression
+gzip compressed data, was "clueai-0.0.2.2.6.tar", last modified: Sat Apr 29 06:37:23 2023, max compression
```

## Comparing `clueai-0.0.2.2.5.tar` & `clueai-0.0.2.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.933634 clueai-0.0.2.2.5/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1063 2022-08-18 02:23:35.000000 clueai-0.0.2.2.5/LICENSE
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:34:49.931882 clueai-0.0.2.2.5/PKG-INFO
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    43545 2023-04-29 06:33:53.000000 clueai-0.0.2.2.5/README.md
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.875434 clueai-0.0.2.2.5/clueai/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      409 2022-11-24 03:00:20.000000 clueai-0.0.2.2.5/clueai/__init__.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1010 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/classify.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    20817 2023-04-29 06:34:10.000000 clueai-0.0.2.2.5/clueai/client.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      371 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/embeddings.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      591 2022-08-19 06:26:56.000000 clueai-0.0.2.2.5/clueai/error.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     2791 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/extract.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1007 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/generation.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      771 2022-09-26 12:05:13.000000 clueai-0.0.2.2.5/clueai/match.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      685 2022-11-25 06:40:19.000000 clueai-0.0.2.2.5/clueai/qa.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      337 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/response.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      434 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/tokenize.py
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.923195 clueai-0.0.2.2.5/clueai.egg-info/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/PKG-INFO
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      373 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/SOURCES.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)        1 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/dependency_links.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)       16 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/requires.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)        7 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/top_level.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)       38 2023-04-29 06:34:49.933846 clueai-0.0.2.2.5/setup.cfg
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1256 2023-04-29 06:34:34.000000 clueai-0.0.2.2.5/setup.py
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:37:23.675325 clueai-0.0.2.2.6/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1063 2022-08-18 02:23:35.000000 clueai-0.0.2.2.6/LICENSE
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:37:23.674756 clueai-0.0.2.2.6/PKG-INFO
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    43545 2023-04-29 06:33:53.000000 clueai-0.0.2.2.6/README.md
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:37:23.650793 clueai-0.0.2.2.6/clueai/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      409 2022-11-24 03:00:20.000000 clueai-0.0.2.2.6/clueai/__init__.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1010 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/classify.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    20923 2023-04-29 06:36:18.000000 clueai-0.0.2.2.6/clueai/client.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      371 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/embeddings.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      591 2022-08-19 06:26:56.000000 clueai-0.0.2.2.6/clueai/error.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     2791 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/extract.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1007 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/generation.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      771 2022-09-26 12:05:13.000000 clueai-0.0.2.2.6/clueai/match.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      685 2022-11-25 06:40:19.000000 clueai-0.0.2.2.6/clueai/qa.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      337 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/response.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      434 2022-08-18 02:13:51.000000 clueai-0.0.2.2.6/clueai/tokenize.py
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:37:23.671985 clueai-0.0.2.2.6/clueai.egg-info/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:37:23.000000 clueai-0.0.2.2.6/clueai.egg-info/PKG-INFO
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      373 2023-04-29 06:37:23.000000 clueai-0.0.2.2.6/clueai.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)        1 2023-04-29 06:37:23.000000 clueai-0.0.2.2.6/clueai.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)       16 2023-04-29 06:37:23.000000 clueai-0.0.2.2.6/clueai.egg-info/requires.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)        7 2023-04-29 06:37:23.000000 clueai-0.0.2.2.6/clueai.egg-info/top_level.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)       38 2023-04-29 06:37:23.675598 clueai-0.0.2.2.6/setup.cfg
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1256 2023-04-29 06:37:21.000000 clueai-0.0.2.2.6/setup.py
```

### Comparing `clueai-0.0.2.2.5/LICENSE` & `clueai-0.0.2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/PKG-INFO` & `clueai-0.0.2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clueai
-Version: 0.0.2.2.5
+Version: 0.0.2.2.6
 Summary: A Python library for the ClueAI API
 Home-page: https://github.com/clue-ai/clueai-python
 Author: matrix
 Author-email: brightmart@hotmail.com
 License: UNKNOWN
 Description: 
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.5 Summary: A Python library
+Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.6 Summary: A Python library
 for the ClueAI API Home-page: https://github.com/clue-ai/clueai-python Author:
 matrix Author-email: brightmart@hotmail.com License: UNKNOWN Description:
 
 
 
            [CLUEAI_logo:_The_data_structure_for_unstructured_data]_
```

### Comparing `clueai-0.0.2.2.5/README.md` & `clueai-0.0.2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/classify.py` & `clueai-0.0.2.2.6/clueai/classify.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/client.py` & `clueai-0.0.2.2.6/clueai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,15 @@
         presence_penalty: float = 0.0,
         stop_sequences: List[str] = None,
         return_likelihoods: str = None,
         headers: dict = {},
         generate_config: dict = {}
     ) -> Generations:
         if len(prompt) > 1024:
+            print(f"警告：你的prompt长度是{len(prompt)}， 超过了1024个字符, 会被截断")
             prompt = prompt[:1024]
         json_body = json.dumps({
             'task_type': "generate",
             'model_name': model_name,
             'input_data': [prompt],
             'num_generations': num_generations,
             'max_tokens': max_tokens,
```

### Comparing `clueai-0.0.2.2.5/clueai/error.py` & `clueai-0.0.2.2.6/clueai/error.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/extract.py` & `clueai-0.0.2.2.6/clueai/extract.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/generation.py` & `clueai-0.0.2.2.6/clueai/generation.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/match.py` & `clueai-0.0.2.2.6/clueai/match.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai/qa.py` & `clueai-0.0.2.2.6/clueai/qa.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.5/clueai.egg-info/PKG-INFO` & `clueai-0.0.2.2.6/clueai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clueai
-Version: 0.0.2.2.5
+Version: 0.0.2.2.6
 Summary: A Python library for the ClueAI API
 Home-page: https://github.com/clue-ai/clueai-python
 Author: matrix
 Author-email: brightmart@hotmail.com
 License: UNKNOWN
 Description: 
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.5 Summary: A Python library
+Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.6 Summary: A Python library
 for the ClueAI API Home-page: https://github.com/clue-ai/clueai-python Author:
 matrix Author-email: brightmart@hotmail.com License: UNKNOWN Description:
 
 
 
            [CLUEAI_logo:_The_data_structure_for_unstructured_data]_
```

### Comparing `clueai-0.0.2.2.5/setup.py` & `clueai-0.0.2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 setuptools.setup(
     name='clueai',
-    version='0.0.2.2.5',
+    version='0.0.2.2.6',
     author='matrix',
     author_email='brightmart@hotmail.com',
     description='A Python library for the ClueAI API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/clue-ai/clueai-python',
     packages=setuptools.find_packages(),
```


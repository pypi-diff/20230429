# Comparing `tmp/feiticeiro_tec-1.0.0.tar.gz` & `tmp/feiticeiro_tec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiticeiro_tec-1.0.0.tar", last modified: Sat Apr 29 05:11:21 2023, max compression
+gzip compressed data, was "feiticeiro_tec-1.0.1.tar", last modified: Sat Apr 29 05:20:11 2023, max compression
```

## Comparing `feiticeiro_tec-1.0.0.tar` & `feiticeiro_tec-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      455 2023-04-29 05:04:44.000000 feiticeiro_tec-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.154599 feiticeiro_tec-1.0.0/feiticeiro_tec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/api/
--rw-r--r--   0 root         (0) root         (0)      193 2023-04-29 04:43:04.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:23:01.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/api/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/api/v1/usuario/
--rw-r--r--   0 root         (0) root         (0)      193 2023-04-29 03:24:23.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/api/v1/usuario/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/create/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/create/app.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/create/model.py
--rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/create/namespace.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-29 04:40:54.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/create/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/database/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec/database/models/
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 04:42:46.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/database/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-29 04:11:43.000000 feiticeiro_tec-1.0.0/feiticeiro_tec/database/models/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-29 05:11:21.000000 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-29 05:11:21.000000 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 05:11:21.000000 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-29 05:11:21.000000 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-29 05:11:21.000000 feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 05:11:21.158599 feiticeiro_tec-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      997 2023-04-29 05:07:34.000000 feiticeiro_tec-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      455 2023-04-29 05:04:44.000000 feiticeiro_tec-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:10:34.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 04:44:22.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/api/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-29 04:43:04.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:23:01.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/api/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/api/v1/usuario/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-29 03:24:23.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/api/v1/usuario/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/create/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/create/app.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/create/model.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/create/namespace.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-29 04:40:54.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/create/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/database/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec/database/models/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 04:42:46.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/database/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-29 04:11:43.000000 feiticeiro_tec-1.0.1/feiticeiro_tec/database/models/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-29 05:20:11.000000 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      647 2023-04-29 05:20:11.000000 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 05:20:11.000000 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-29 05:20:11.000000 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-29 05:20:11.000000 feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 05:20:11.684298 feiticeiro_tec-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 05:20:09.000000 feiticeiro_tec-1.0.1/setup.py
```

### Comparing `feiticeiro_tec-1.0.0/PKG-INFO` & `feiticeiro_tec-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiticeiro_tec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
```

### Comparing `feiticeiro_tec-1.0.0/feiticeiro_tec/create/namespace.py` & `feiticeiro_tec-1.0.1/feiticeiro_tec/create/namespace.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.0.0/feiticeiro_tec/create/server.py` & `feiticeiro_tec-1.0.1/feiticeiro_tec/create/server.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.0.0/feiticeiro_tec/database/models/base.py` & `feiticeiro_tec-1.0.1/feiticeiro_tec/database/models/base.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/PKG-INFO` & `feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiticeiro-tec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
```

### Comparing `feiticeiro_tec-1.0.0/feiticeiro_tec.egg-info/SOURCES.txt` & `feiticeiro_tec-1.0.1/feiticeiro_tec.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 README.md
 setup.py
+feiticeiro_tec/__init__.py
+feiticeiro_tec/__main__.py
 feiticeiro_tec.egg-info/PKG-INFO
 feiticeiro_tec.egg-info/SOURCES.txt
 feiticeiro_tec.egg-info/dependency_links.txt
 feiticeiro_tec.egg-info/requires.txt
 feiticeiro_tec.egg-info/top_level.txt
 feiticeiro_tec/api/__init__.py
 feiticeiro_tec/api/v1/__init__.py
```

### Comparing `feiticeiro_tec-1.0.0/setup.py` & `feiticeiro_tec-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 
 import os
 
 
 def listar_subpastas(diretorio):
-    subpastas = []
+    subpastas = [diretorio]
     for nome in os.listdir(diretorio):
         caminho = os.path.join(diretorio, nome)
         if os.path.isdir(caminho):
             subpastas.append(caminho)
             subpastas.extend(listar_subpastas(caminho))
     return subpastas
 
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='feiticeiro_tec',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/feiticeiro-tec/feiticeiro-tec',
     license='BSD3',
     author='Silvio Henrique Cruz Da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silviohenriquecruzdasilva@gmail.com',
     keywords='Pacote',
```


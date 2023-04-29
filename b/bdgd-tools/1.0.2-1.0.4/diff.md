# Comparing `tmp/bdgd_tools-1.0.2.tar.gz` & `tmp/bdgd_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdgd_tools-1.0.2.tar", last modified: Sat Apr 22 13:51:42 2023, max compression
+gzip compressed data, was "bdgd_tools-1.0.4.tar", last modified: Sat Apr 29 21:21:02 2023, max compression
```

## Comparing `bdgd_tools-1.0.2.tar` & `bdgd_tools-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools/gui/
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/gui/GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/bdgd_tools/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/BusCoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Capacitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Count_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/LineCode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/Loadshape.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/bdgd_tools/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/sample/Sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/bdgd_tools/sample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.531063 bdgd_tools-1.0.2/bdgd_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 13:51:42.000000 bdgd_tools-1.0.2/bdgd_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 13:51:41.000000 bdgd_tools-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:51:42.535063 bdgd_tools-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-22 13:51:39.000000 bdgd_tools-1.0.2/tests/test_bdgd_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/core/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/gui/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/BusCoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Count_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/LineCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/Loadshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/sample/Sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/bdgd_tools/sample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/bdgd_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-29 21:21:02.000000 bdgd_tools-1.0.4/bdgd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 21:21:02.000000 bdgd_tools-1.0.4/bdgd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:21:02.000000 bdgd_tools-1.0.4/bdgd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:21:02.000000 bdgd_tools-1.0.4/bdgd_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 21:21:02.000000 bdgd_tools-1.0.4/bdgd_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-29 21:21:02.845678 bdgd_tools-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-29 21:21:01.000000 bdgd_tools-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:21:02.841678 bdgd_tools-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 21:20:56.000000 bdgd_tools-1.0.4/tests/test_bdgd_tools.py
```

### Comparing `bdgd_tools-1.0.2/CONTRIBUTING.rst` & `bdgd_tools-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/HISTORY.rst` & `bdgd_tools-1.0.4/HISTORY.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+1.0.4(2023-04-29)
+------------------
+
+* Backend modifications to run properly auto publish and readthedocs.
+
 1.0.1(2023-04-22)
 ------------------
 
 * Backend modifications to run properly auto publish and readthedocs.
 
 1.0.0(2023-03-22)
 ------------------
```

### Comparing `bdgd_tools-1.0.2/LICENSE` & `bdgd_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/PKG-INFO` & `bdgd_tools-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdgd_tools
-Version: 1.0.2
+Version: 1.0.4
 Summary: Short description
 Home-page: https://github.com/eniocc/bdgd_tools
 Author: Ênio Rodrigues
 Author-email: eniocc@gmail.com
 License: MIT license
 Keywords: bdgd_tools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -77,14 +77,19 @@
 
 
 
 =======
 History
 =======
 
+1.0.4(2023-04-29)
+------------------
+
+* Backend modifications to run properly auto publish and readthedocs.
+
 1.0.1(2023-04-22)
 ------------------
 
 * Backend modifications to run properly auto publish and readthedocs.
 
 1.0.0(2023-03-22)
 ------------------
```

### Comparing `bdgd_tools-1.0.2/README.rst` & `bdgd_tools-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/core/Core.py` & `bdgd_tools-1.0.4/bdgd_tools/core/Core.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,19 @@
  * Time: 12:02
 """
 import inspect
 import json
 import os.path
 import pathlib
 import time
+from typing import Optional
+
 import geopandas as gpd
 
-from bdgd_tools import Sample, Case
+from bdgd_tools import Sample, Case, Circuit, LineCode
 from bdgd_tools.core.Utils import load_json
 from bdgd_tools.gui.GUI import GUI
 
 
 class Table:
     def __init__(self, name, columns, data_types, ignore_geometry_):
         self.name = name
@@ -31,57 +33,108 @@
     def __str__(self):
         return f"Table(name={self.name}, columns={self.columns}, data_types={self.data_types}, " \
                f"ignore_geometry={self.ignore_geometry})"
 
 
 class JsonData:
     def __init__(self, file_name):
+        """
+        Inicializa a classe JsonData com o nome do arquivo de entrada.
+
+        :param file_name: Nome do arquivo JSON de entrada.
+        """
         self.data = self._read_json_file(file_name)
         self.tables = self._create_tables()
 
-    def _read_json_file(self, file_name):
+    @staticmethod
+    def _read_json_file(file_name):
+        """
+        Lê o arquivo JSON fornecido e retorna o conteúdo como um objeto Python.
+
+        :param file_name: Nome do arquivo JSON de entrada.
+        :return: Objeto Python contendo o conteúdo do arquivo JSON.
+        """
         with open(file_name, 'r', encoding='utf-8') as file:
             data = json.load(file)
         return data
 
     def _create_tables(self):
-        tables = {}
-        for table_name, table_data in self.data["configuration"]["tables"].items():
-            tables[table_name] = Table(table_name, table_data["columns"], table_data["type"],
-                                       table_data["ignore_geometry"])
-        return tables
+        """
+        Cria um dicionário de tabelas a partir dos dados carregados do arquivo JSON.
+
+        :return: Dicionário contendo informações das tabelas a serem processadas.
+        """
+        return {
+            table_name: Table(
+                table_name,
+                table_data["columns"],
+                table_data["type"],
+                table_data["ignore_geometry"],
+            )
+            for table_name, table_data in self.data["configuration"][
+                "tables"
+            ].items()
+        }
 
     def get_tables(self):
+        """
+        Retorna o dicionário de tabelas.
+
+        :return: Dicionário contendo informações das tabelas a serem processadas.
+        """
         return self.tables
 
-    def convert_data_types(self, df, column_types):
+    @staticmethod
+    def convert_data_types(df, column_types):
+        """
+        Converte os tipos de dados das colunas do DataFrame fornecido.
+
+        :param df: DataFrame a ser processado.
+        :param column_types: Dicionário contendo mapeamento de colunas para tipos de dados.
+        :return: DataFrame com tipos de dados convertidos.
+        """
         return df.astype(column_types)
 
     def create_geodataframes(self, file_name, runs=1):
+        """
+        Cria GeoDataFrames a partir de um arquivo de entrada e coleta estatísticas.
+
+        :param file_name: Nome do arquivo de entrada.
+        :param runs: Número de vezes que cada tabela será carregada e convertida (padrão: 1).
+        :return: Dicionário contendo GeoDataFrames e estatísticas.
+        """
         geodataframes = {}
-        gdf_converted = None
+
         for table_name, table in self.tables.items():
             load_times = []
             conversion_times = []
+            gdf_converted = None
+
             for _ in range(runs):
                 start_time = time.time()
                 gdf_ = gpd.read_file(file_name, layer=table.name, include_fields=table.columns,
                                      ignore_geometry=table.ignore_geometry)
                 start_conversion_time = time.time()
                 gdf_converted = self.convert_data_types(gdf_, table.data_types)
                 end_time = time.time()
+
                 load_times.append(start_conversion_time - start_time)
                 conversion_times.append(end_time - start_conversion_time)
 
             load_time_avg = sum(load_times) / len(load_times)
             conversion_time_avg = sum(conversion_times) / len(conversion_times)
             mem_usage = gdf_converted.memory_usage(index=True, deep=True).sum() / 1024 ** 2
 
-            geodataframes[table_name] = [
-                gdf_converted, mem_usage, load_time_avg, conversion_time_avg, table.ignore_geometry]
+            geodataframes[table_name] = {
+                'gdf': gdf_converted,
+                'memory_usage': mem_usage,
+                'load_time_avg': load_time_avg,
+                'conversion_time_avg': conversion_time_avg,
+                'ignore_geometry': table.ignore_geometry
+            }
         return geodataframes
 
 
 def get_caller_directory(caller_frame: inspect) -> pathlib.Path:
     """
     Returns the file directory that calls this function.
 
@@ -100,21 +153,25 @@
     print(f"Base escolhida {folder_bdgd}")
     data = load_json(json_file=json_file)
 
     gui = GUI(folder_bdgd, data)
     gui.load_window()
 
 
-def run() -> None:
+def run(folder: Optional[str] = None) -> None:
     case = Case()
     s = Sample()
-    folder_bdgd = s.mux_energia
+    folder_bdgd = folder or s.mux_energia
     json_file_name = os.path.join(os.getcwd(), "bdgd2dss.json")
 
     json_data = JsonData(json_file_name)
 
     geodataframes = json_data.create_geodataframes(folder_bdgd)
     case.dfs = geodataframes
-    # for table_name, (gdf, mem_usage, load_time_avg, conversion_time_avg, ignore_geometry) in case.dfs.items():
-    #     print(
-    #         f"{table_name}; {mem_usage:.4f}; {load_time_avg:.4f} ; {conversion_time_avg:.4f}; {ignore_geometry}; "
-    #         f"SPECIFIC")
+
+    case.circuitos = Circuit.create_circuit_from_json(json_data.data, case.dfs['CTMT']['gdf'])
+    for c in case.circuitos:
+        print(c)
+
+    case.line_codes = LineCode.create_linecode_from_json(json_data.data, case.dfs['SEGCON']['gdf'])
+    for l_ in case.line_codes:
+        print(l_)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bdgd_tools-1.0.2/bdgd_tools/core/Utils.py` & `bdgd_tools-1.0.4/bdgd_tools/core/Utils.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/gui/GUI.py` & `bdgd_tools-1.0.4/bdgd_tools/gui/GUI.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/BusCoords.py` & `bdgd_tools-1.0.4/bdgd_tools/model/BusCoords.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/Capacitor.py` & `bdgd_tools-1.0.4/bdgd_tools/model/Capacitor.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/Case.py` & `bdgd_tools-1.0.4/bdgd_tools/model/Case.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,32 +6,39 @@
  * Time: 10:05
  *
  * Edited by: eniocc
  * Date: 27/03/2023
  * Time: 10:05
 """
 from dataclasses import dataclass, field
-import geopandas as gpd
 from bdgd_tools import Circuit, LineCode
 
 
 @dataclass
 class Case:
     _circuitos: list[Circuit] = field(init=False)
     _line_codes: list[LineCode] = field(init=False)
     _dfs: dict = field(init=False)
 
     @property
     def circuitos(self):
         return self._circuitos
 
+    @circuitos.setter
+    def circuitos(self, value):
+        self._circuitos = value
+
     @property
     def line_codes(self):
         return self._line_codes
 
+    @line_codes.setter
+    def line_codes(self, value):
+        self._line_codes = value
+
     @property
     def dfs(self):
         return self._dfs
 
     @dfs.setter
     def dfs(self, value: dict):
         self._dfs = value
```

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/Count_days.py` & `bdgd_tools-1.0.4/bdgd_tools/model/Count_days.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/LineCode.py` & `bdgd_tools-1.0.4/bdgd_tools/model/LineCode.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/model/Loadshape.py` & `bdgd_tools-1.0.4/bdgd_tools/model/Loadshape.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools/sample/Sample.py` & `bdgd_tools-1.0.4/bdgd_tools/sample/Sample.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/bdgd_tools.egg-info/PKG-INFO` & `bdgd_tools-1.0.4/bdgd_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdgd-tools
-Version: 1.0.2
+Version: 1.0.4
 Summary: Short description
 Home-page: https://github.com/eniocc/bdgd_tools
 Author: Ênio Rodrigues
 Author-email: eniocc@gmail.com
 License: MIT license
 Keywords: bdgd_tools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -77,14 +77,19 @@
 
 
 
 =======
 History
 =======
 
+1.0.4(2023-04-29)
+------------------
+
+* Backend modifications to run properly auto publish and readthedocs.
+
 1.0.1(2023-04-22)
 ------------------
 
 * Backend modifications to run properly auto publish and readthedocs.
 
 1.0.0(2023-03-22)
 ------------------
```

### Comparing `bdgd_tools-1.0.2/bdgd_tools.egg-info/SOURCES.txt` & `bdgd_tools-1.0.4/bdgd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/docs/Makefile` & `bdgd_tools-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/docs/conf.py` & `bdgd_tools-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/docs/installation.rst` & `bdgd_tools-1.0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/docs/make.bat` & `bdgd_tools-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bdgd_tools-1.0.2/setup.py` & `bdgd_tools-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     include_package_data=True,
     keywords='bdgd_tools',
     name='bdgd_tools',
     packages=find_packages(include=['bdgd_tools', 'bdgd_tools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eniocc/bdgd_tools',
-    version='1.0.2',
+    version='1.0.4',
     zip_safe=False,
 )
```


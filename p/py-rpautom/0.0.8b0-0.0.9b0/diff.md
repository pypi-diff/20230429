# Comparing `tmp/py-rpautom-0.0.8b0.tar.gz` & `tmp/py-rpautom-0.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-rpautom-0.0.8b0.tar", last modified: Mon Jan 16 14:18:56 2023, max compression
+gzip compressed data, was "py-rpautom-0.0.9b0.tar", last modified: Wed Jan 18 11:25:15 2023, max compression
```

## Comparing `py-rpautom-0.0.8b0.tar` & `py-rpautom-0.0.9b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 14:18:56.865759 py-rpautom-0.0.8b0/
--rw-rw-rw-   0        0        0    35823 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/LICENSE
--rw-rw-rw-   0        0        0     2099 2023-01-16 14:18:56.865759 py-rpautom-0.0.8b0/PKG-INFO
--rw-rw-rw-   0        0        0     1397 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-16 14:18:56.818873 py-rpautom-0.0.8b0/py_rpautom/
--rw-rw-rw-   0        0        0        0 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/py_rpautom/__init__.py
--rw-rw-rw-   0        0        0    21504 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/py_rpautom/desktop_utils.py
--rw-rw-rw-   0        0        0    29480 2023-01-16 13:55:29.000000 py-rpautom-0.0.8b0/py_rpautom/python_utils.py
--rw-rw-rw-   0        0        0    48420 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/py_rpautom/web_utils.py
-drwxrwxrwx   0        0        0        0 2023-01-16 14:18:56.850134 py-rpautom-0.0.8b0/py_rpautom.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-01-16 14:18:56.000000 py-rpautom-0.0.8b0/py_rpautom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-01-16 14:18:56.000000 py-rpautom-0.0.8b0/py_rpautom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 14:18:56.000000 py-rpautom-0.0.8b0/py_rpautom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-01-16 14:18:56.000000 py-rpautom-0.0.8b0/py_rpautom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-16 14:18:56.000000 py-rpautom-0.0.8b0/py_rpautom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-16 14:18:56.865759 py-rpautom-0.0.8b0/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-01-16 14:15:11.000000 py-rpautom-0.0.8b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-16 14:18:56.850134 py-rpautom-0.0.8b0/tests/
--rw-rw-rw-   0        0        0        0 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/tests/__init__.py
--rw-rw-rw-   0        0        0     9086 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/tests/conftest.py
--rw-rw-rw-   0        0        0     6186 2023-01-06 18:14:15.000000 py-rpautom-0.0.8b0/tests/test_desktop_utils.py
+drwxrwxrwx   0        0        0        0 2023-01-18 11:25:15.556657 py-rpautom-0.0.9b0/
+-rw-rw-rw-   0        0        0    35823 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/LICENSE
+-rw-rw-rw-   0        0        0     2099 2023-01-18 11:25:15.556657 py-rpautom-0.0.9b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1397 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/README.md
+drwxrwxrwx   0        0        0        0 2023-01-18 11:25:15.508614 py-rpautom-0.0.9b0/py_rpautom/
+-rw-rw-rw-   0        0        0        0 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/py_rpautom/__init__.py
+-rw-rw-rw-   0        0        0    21504 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/py_rpautom/desktop_utils.py
+-rw-rw-rw-   0        0        0    29480 2023-01-16 13:55:29.000000 py-rpautom-0.0.9b0/py_rpautom/python_utils.py
+-rw-rw-rw-   0        0        0    48420 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/py_rpautom/web_utils.py
+drwxrwxrwx   0        0        0        0 2023-01-18 11:25:15.540618 py-rpautom-0.0.9b0/py_rpautom.egg-info/
+-rw-rw-rw-   0        0        0     2099 2023-01-18 11:25:15.000000 py-rpautom-0.0.9b0/py_rpautom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-01-18 11:25:15.000000 py-rpautom-0.0.9b0/py_rpautom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-18 11:25:15.000000 py-rpautom-0.0.9b0/py_rpautom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-01-18 11:25:15.000000 py-rpautom-0.0.9b0/py_rpautom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-01-18 11:25:15.000000 py-rpautom-0.0.9b0/py_rpautom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-18 11:25:15.556657 py-rpautom-0.0.9b0/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2023-01-18 11:22:48.000000 py-rpautom-0.0.9b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-18 11:25:15.550644 py-rpautom-0.0.9b0/tests/
+-rw-rw-rw-   0        0        0        0 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/tests/__init__.py
+-rw-rw-rw-   0        0        0     9086 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/tests/conftest.py
+-rw-rw-rw-   0        0        0     6186 2023-01-06 18:14:15.000000 py-rpautom-0.0.9b0/tests/test_desktop_utils.py
```

### Comparing `py-rpautom-0.0.8b0/LICENSE` & `py-rpautom-0.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/PKG-INFO` & `py-rpautom-0.0.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-rpautom
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: Conjunto de utilitários para automação de processos.
 Home-page: https://github.com/aranseiki/py-rpautom/
 Author: aranseiki
 Author-email: techall@hotmail.com.br
 Project-URL: Py-RPAutom, https://github.com/aranseiki/py-rpautom/
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `py-rpautom-0.0.8b0/README.md` & `py-rpautom-0.0.9b0/README.md`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/py_rpautom/desktop_utils.py` & `py-rpautom-0.0.9b0/py_rpautom/desktop_utils.py`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/py_rpautom/python_utils.py` & `py-rpautom-0.0.9b0/py_rpautom/python_utils.py`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/py_rpautom/web_utils.py` & `py-rpautom-0.0.9b0/py_rpautom/web_utils.py`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/py_rpautom.egg-info/PKG-INFO` & `py-rpautom-0.0.9b0/py_rpautom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-rpautom
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: Conjunto de utilitários para automação de processos.
 Home-page: https://github.com/aranseiki/py-rpautom/
 Author: aranseiki
 Author-email: techall@hotmail.com.br
 Project-URL: Py-RPAutom, https://github.com/aranseiki/py-rpautom/
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `py-rpautom-0.0.8b0/setup.py` & `py-rpautom-0.0.9b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 base_dir = os.path.dirname(__file__)
 
 with open(os.path.join(base_dir, "README.md"), encoding='utf8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="py-rpautom",
-    version="0.0.8b",
+    version="0.0.9b",
     author="aranseiki",
     author_email="techall@hotmail.com.br",
     description="Conjunto de utilitários para automação de processos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aranseiki/py-rpautom/",
     packages=setuptools.find_packages(),
@@ -36,9 +36,10 @@
         'pywin32',
         'PyMuPDF',
         'PyPDF2',
         'Pytesseract',
         'requests',
         'selenium',
         'urllib3',
+        'xlrd',
     ]
 )
```

### Comparing `py-rpautom-0.0.8b0/tests/conftest.py` & `py-rpautom-0.0.9b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py-rpautom-0.0.8b0/tests/test_desktop_utils.py` & `py-rpautom-0.0.9b0/tests/test_desktop_utils.py`

 * *Files identical despite different names*


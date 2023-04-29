# Comparing `tmp/mdutils-1.5.1.tar.gz` & `tmp/mdutils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdutils-1.5.1.tar", last modified: Sat Mar 11 16:21:09 2023, max compression
+gzip compressed data, was "mdutils-1.6.0.tar", last modified: Sat Apr 29 14:36:12 2023, max compression
```

## Comparing `mdutils-1.5.1.tar` & `mdutils-1.6.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.449509 mdutils-1.5.1/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     1071 2022-12-10 13:26:39.000000 mdutils-1.5.1/LICENSE.txt
--rw-r--r--   0 didaccollpujals   (501) staff       (20)      100 2022-12-10 13:26:39.000000 mdutils-1.5.1/MANIFEST.in
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3667 2023-03-11 16:21:09.449599 mdutils-1.5.1/PKG-INFO
--rw-r--r--   0 didaccollpujals   (501) staff       (20)    14615 2022-12-12 08:01:49.000000 mdutils-1.5.1/README.md
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.446101 mdutils-1.5.1/doc/
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.447031 mdutils-1.5.1/doc/source/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     2079 2022-12-12 08:01:49.000000 mdutils-1.5.1/doc/source/README.rst
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.447244 mdutils-1.5.1/mdutils/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)      196 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/__init__.py
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.448226 mdutils-1.5.1/mdutils/fileutils/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)       53 2022-12-10 13:26:39.000000 mdutils-1.5.1/mdutils/fileutils/__init__.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3373 2023-03-11 16:15:29.000000 mdutils-1.5.1/mdutils/fileutils/fileutils.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)    21744 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/mdutils.py
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.449394 mdutils-1.5.1/mdutils/tools/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     7511 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/Header.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3187 2022-12-10 13:26:39.000000 mdutils-1.5.1/mdutils/tools/Html.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     1744 2022-12-10 13:26:39.000000 mdutils-1.5.1/mdutils/tools/Image.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3013 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/Link.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3606 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/MDList.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     4593 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/Table.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     2293 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/TableOfContents.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     5236 2022-12-10 13:26:39.000000 mdutils-1.5.1/mdutils/tools/TextUtils.py
--rw-r--r--   0 didaccollpujals   (501) staff       (20)      244 2022-12-12 08:01:49.000000 mdutils-1.5.1/mdutils/tools/__init__.py
-drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-03-11 16:21:09.447823 mdutils-1.5.1/mdutils.egg-info/
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     3667 2023-03-11 16:21:09.000000 mdutils-1.5.1/mdutils.egg-info/PKG-INFO
--rw-r--r--   0 didaccollpujals   (501) staff       (20)      554 2023-03-11 16:21:09.000000 mdutils-1.5.1/mdutils.egg-info/SOURCES.txt
--rw-r--r--   0 didaccollpujals   (501) staff       (20)        1 2023-03-11 16:21:09.000000 mdutils-1.5.1/mdutils.egg-info/dependency_links.txt
--rw-r--r--   0 didaccollpujals   (501) staff       (20)        1 2023-02-11 22:40:25.000000 mdutils-1.5.1/mdutils.egg-info/not-zip-safe
--rw-r--r--   0 didaccollpujals   (501) staff       (20)        8 2023-03-11 16:21:09.000000 mdutils-1.5.1/mdutils.egg-info/top_level.txt
--rw-r--r--   0 didaccollpujals   (501) staff       (20)      159 2023-03-11 16:21:09.449832 mdutils-1.5.1/setup.cfg
--rw-r--r--   0 didaccollpujals   (501) staff       (20)     1420 2023-03-11 16:16:06.000000 mdutils-1.5.1/setup.py
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.073740 mdutils-1.6.0/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     1071 2022-12-10 13:26:39.000000 mdutils-1.6.0/LICENSE.txt
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)      100 2022-12-10 13:26:39.000000 mdutils-1.6.0/MANIFEST.in
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3222 2023-04-29 14:36:12.073804 mdutils-1.6.0/PKG-INFO
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)    14678 2023-04-29 14:30:53.000000 mdutils-1.6.0/README.md
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.069025 mdutils-1.6.0/doc/
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.070133 mdutils-1.6.0/doc/source/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     2165 2023-04-29 14:30:53.000000 mdutils-1.6.0/doc/source/README.rst
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.070471 mdutils-1.6.0/mdutils/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)      196 2022-12-12 08:01:49.000000 mdutils-1.6.0/mdutils/__init__.py
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.071642 mdutils-1.6.0/mdutils/fileutils/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)       53 2022-12-10 13:26:39.000000 mdutils-1.6.0/mdutils/fileutils/__init__.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3499 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/fileutils/fileutils.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)    23463 2023-04-27 12:11:46.000000 mdutils-1.6.0/mdutils/mdutils.py
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.073264 mdutils-1.6.0/mdutils/tools/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     7689 2023-04-27 12:11:46.000000 mdutils-1.6.0/mdutils/tools/Header.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3351 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/Html.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     1845 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/Image.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3223 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/Link.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3765 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/MDList.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     4637 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/Table.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     2607 2023-04-27 12:11:50.000000 mdutils-1.6.0/mdutils/tools/TableOfContents.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     5602 2023-03-30 17:48:21.000000 mdutils-1.6.0/mdutils/tools/TextUtils.py
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)      244 2022-12-12 08:01:49.000000 mdutils-1.6.0/mdutils/tools/__init__.py
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.071321 mdutils-1.6.0/mdutils.egg-info/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     3222 2023-04-29 14:36:12.000000 mdutils-1.6.0/mdutils.egg-info/PKG-INFO
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)      591 2023-04-29 14:36:12.000000 mdutils-1.6.0/mdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)        1 2023-04-29 14:36:12.000000 mdutils-1.6.0/mdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)        1 2023-02-11 22:40:25.000000 mdutils-1.6.0/mdutils.egg-info/not-zip-safe
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)        8 2023-04-29 14:36:12.000000 mdutils-1.6.0/mdutils.egg-info/top_level.txt
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     1201 2023-04-29 14:32:31.000000 mdutils-1.6.0/pyproject.toml
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)      159 2023-04-29 14:36:12.073988 mdutils-1.6.0/setup.cfg
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)     1420 2023-04-29 14:32:31.000000 mdutils-1.6.0/setup.py
+drwxr-xr-x   0 didaccollpujals   (501) staff       (20)        0 2023-04-29 14:36:12.073479 mdutils-1.6.0/tests/
+-rw-r--r--   0 didaccollpujals   (501) staff       (20)    18466 2023-03-30 17:48:21.000000 mdutils-1.6.0/tests/test_mdutils.py
```

### Comparing `mdutils-1.5.1/LICENSE.txt` & `mdutils-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdutils-1.5.1/PKG-INFO` & `mdutils-1.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,106 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdutils
-Version: 1.5.1
+Version: 1.6.0
 Summary: Useful package for creating Markdown files while executing python code.
 Home-page: https://github.com/didix21/mdutils
 Author: Didac Coll
 Author-email: didaccoll_93@hotmail.com
 Maintainer: Didac Coll
 Maintainer-email: didaccoll_93@hotmail.com
 License: MIT
 Project-URL: Documentation, http://mdutils.readthedocs.io
 Project-URL: Say Thanks!, https://github.com/didix21/
 Project-URL: Source, https://github.com/didix21/mdutils
-Description: =======
-        mdutils
-        =======
-        |build-status| |documentation-status| |coverage-status|
-        
-        .. contents:: Table of Contents
-        
-        Overview
-        ========
-        This Python package contains a set of basic tools that can help to create a markdown file while running a Python code.
-        Thus, if you are executing a Python code and you save the result in a text file, Why not format it? So
-        using files such as Markdown can give a great look to those results. In this way, mdutils will make things easy for
-        creating Markdown files.
-        
-        - Project Homepage: https://github.com/didix21/mdutils
-        - Download Page: https://pypi.python.org/pypi/mdutils
-        - Documentation: http://mdutils.readthedocs.io/en/latest/
-        
-        MIT License, (C) 2018 Didac Coll <didaccoll_93@hotmail.com>
-        
-        Features
-        ========
-        There are some different features available on that version of mdutils:
-        
-        Writing and Reading Files
-        -------------------------
-        - Write and Read Markdown files.
-        - Append data to the end of a Markdown file.
-        - Use markers to place text.
-        
-        Markdown
-        --------
-        - Implemented method to give format to the text: bold, italics, change color...
-        - Align text.
-        - Add headers of levels 1 til 6 (atx style) or 1 and 2 (setext style).
-        - Create tables.
-        - Create a table of contents.
-        - Add Links.
-        - Add Lists.
-        - Add Markdown Images.
-        - Add Html Images.
-        
-        .. note::
-        
-            Some available features will depen on which CSS you are using. For example, GitHub do not allows to give color to text.
-        
-        
-        Installation
-        ============
-        Use pip to install mdutils:
-        
-        .. code:: bash
-        
-            $ pip install mdutils
-        
-        
-        
-        .. |build-status| image:: https://travis-ci.org/didix21/mdutils.svg?branch=master
-            :target: https://travis-ci.org/didix21/mdutils
-            :alt: Build Status
-        
-        .. |documentation-status| image:: https://readthedocs.org/projects/mdutils/badge/?version=latest
-            :target: http://mdutils.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. |coverage-status| image:: https://coveralls.io/repos/github/didix21/mdutils/badge.svg?branch=add-coveralls
-            :target: https://coveralls.io/github/didix21/mdutils?branch=add-coveralls
-            :alt: Coverage Status
-        
 Platform: Python 3.6
 Platform: Python 3.7
 Platform: Python 3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.txt
+
+=======
+mdutils
+=======
+|build-status| |documentation-status| |coverage-status|
+
+.. contents:: Table of Contents
+
+Overview
+========
+This Python package contains a set of basic tools that can help to create a markdown file while running a Python code.
+Thus, if you are executing a Python code and you save the result in a text file, Why not format it? So
+using files such as Markdown can give a great look to those results. In this way, mdutils will make things easy for
+creating Markdown files.
+
+- Project Homepage: https://github.com/didix21/mdutils
+- Download Page: https://pypi.python.org/pypi/mdutils
+- Documentation: http://mdutils.readthedocs.io/en/latest/
+
+MIT License, (C) 2018 Didac Coll <didaccoll_93@hotmail.com>
+
+Features
+========
+There are some different features available on that version of mdutils:
+
+Writing and Reading Files
+-------------------------
+- Write and Read Markdown files.
+- Append data to the end of a Markdown file.
+- Use markers to place text.
+
+Markdown
+--------
+- Implemented method to give format to the text: bold, italics, change color...
+- Align text.
+- Add headers of levels 1 til 6 (atx style) or 1 and 2 (setext style).
+- Create tables.
+- Create a table of contents.
+- Add Links.
+- Add Lists.
+- Add Markdown Images.
+- Add Html Images.
+
+.. note::
+
+    Some available features will depen on which CSS you are using. For example, GitHub do not allows to give color to text.
+
+
+Installation
+============
+
+Pip
+---
+Use pip to install mdutils:
+
+.. code:: bash
+
+    $ pip install mdutils
+
+Poetry
+------
+Use poetry to install mdutils:
+
+.. code:: bash
+
+    $ poetry add mdutils
+
+
+.. |build-status| image:: https://github.com/didix21/mdutils/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/didix21/mdutils
+    :alt: Build Status
+
+.. |documentation-status| image:: https://readthedocs.org/projects/mdutils/badge/?version=latest
+    :target: http://mdutils.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |coverage-status| image:: https://codecov.io/gh/didix21/mdutils/branch/master/graph/badge.svg?token=0DN72Z1B6V
+    :target: https://codecov.io/gh/didix21/mdutils
+    :alt: Coverage Status
```

### Comparing `mdutils-1.5.1/README.md` & `mdutils-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mdutils
-[![Build Status](https://travis-ci.org/didix21/mdutils.svg?branch=master)](https://travis-ci.org/didix21/mdutils)
+![Build Status](https://github.com/didix21/mdutils/actions/workflows/main.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/mdutils/badge/?version=latest)](http://mdutils.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/didix21/mdutils/branch/master/graph/badge.svg?token=0DN72Z1B6V)](https://codecov.io/gh/didix21/mdutils)
 
 Table of Contents
 =================
 - [Overview](#overview)
 - [Features](#features)
@@ -47,19 +47,29 @@
 - Add Markdown Images.
 - Add Html Images.
 
 **NOTE:** some available features will depend on which CSS you are using. For example, GitHub does not allow to give color to text.
 
 Installation
 ============
+
+Pip
+---
 Use pip to install mdutils:
 ```bash
 $ pip install mdutils
 ```
 
+Poetry
+------
+Use poetry to install mdutils:
+```bash
+$ poetry add mdutils
+```
+
 Markdown File Example
 =====================
 
 Contents
 ========
 
 * [Overview](#overview)
```

### Comparing `mdutils-1.5.1/doc/source/README.rst` & `mdutils-1.6.0/doc/source/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -43,26 +43,36 @@
 .. note::
 
     Some available features will depen on which CSS you are using. For example, GitHub do not allows to give color to text.
 
 
 Installation
 ============
+
+Pip
+---
 Use pip to install mdutils:
 
 .. code:: bash
 
     $ pip install mdutils
 
+Poetry
+------
+Use poetry to install mdutils:
+
+.. code:: bash
+
+    $ poetry add mdutils
 
 
-.. |build-status| image:: https://travis-ci.org/didix21/mdutils.svg?branch=master
-    :target: https://travis-ci.org/didix21/mdutils
+.. |build-status| image:: https://github.com/didix21/mdutils/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/didix21/mdutils
     :alt: Build Status
 
 .. |documentation-status| image:: https://readthedocs.org/projects/mdutils/badge/?version=latest
     :target: http://mdutils.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |coverage-status| image:: https://coveralls.io/repos/github/didix21/mdutils/badge.svg?branch=add-coveralls
-    :target: https://coveralls.io/github/didix21/mdutils?branch=add-coveralls
+.. |coverage-status| image:: https://codecov.io/gh/didix21/mdutils/branch/master/graph/badge.svg?token=0DN72Z1B6V
+    :target: https://codecov.io/gh/didix21/mdutils
     :alt: Coverage Status
```

### Comparing `mdutils-1.5.1/mdutils/fileutils/fileutils.py` & `mdutils-1.6.0/mdutils/fileutils/fileutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,90 @@
 # Python
 #
 # This module implements a main class that allows to create markdown files, write in them or read.
 #
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2018 Dídac Coll
+from typing import Optional
 
 
 class MarkDownFile(object):
     """MarkDownFile class creates a new file of MarkDown extension.
 
     Features available are:
         - Create a file.
         - Rewrite a file with new data.
         - Write at the end of the file."""
 
-    def __init__(self, name='', dirname: str = None):
+    def __init__(self, name="", dirname: Optional[str] = None):
         """Creates a markdown file, if name is not empty.
         :param str name: provide the file name or a path joinly with the file name. For example: `./my-path/my-file.md`.
-        :param str dirname: use dirname if you want to provide the path separately from the name. 
+        :param str dirname: use dirname if you want to provide the path separately from the name.
         If not you can specify the path directly on the name."""
         if name:
             self.dirname = dirname
             self.file_name = self._get_file_name(name, dirname)
-            self.file = open(f'{self.file_name}', 'w+', encoding='UTF-8')
+            self.file = open(f"{self.file_name}", "w+", encoding="UTF-8")
             self.file.close()
 
-    def _get_file_name(self, name: str, dirname: str = None ) -> str:
-            if dirname:
-                return f'{dirname}/{name}' if name.endswith('.md') else f'{dirname}/{name}.md'
-            
-            return name if name.endswith('.md') else f'{name}.md'
+    def _get_file_name(self, name: str, dirname: Optional[str] = None) -> str:
+        if dirname:
+            return (
+                f"{dirname}/{name}" if name.endswith(".md") else f"{dirname}/{name}.md"
+            )
 
-    def rewrite_all_file(self, data):
+        return name if name.endswith(".md") else f"{name}.md"
+
+    def rewrite_all_file(self, data: str):
         """Rewrite all the data of a Markdown file by ``data``.
 
-        :param str data: is a string containing all the data that is written in the markdown file."""
-        with open(f'{self.file_name}', 'w', encoding='utf-8') as self.file:
+        :param str data: is a string containing all the data that is written in the markdown file.
+        """
+        with open(f"{self.file_name}", "w", encoding="utf-8") as self.file:
             self.file.write(data)
 
-    def append_end(self, data):
+    def append_end(self, data: str):
         """Write at the last position of a Markdown file.
 
-        :param str data: is a string containing all the data that is written in the markdown file."""
-        with open(f'{self.file_name}', 'a', encoding='utf-8') as self.file:
+        :param str data: is a string containing all the data that is written in the markdown file.
+        """
+        with open(f"{self.file_name}", "a", encoding="utf-8") as self.file:
             self.file.write(data)
 
-    def append_after_second_line(self, data):
+    def append_after_second_line(self, data: str):
         """Write after the file's first line.
 
-        :param str data: is a string containing all the data that is written in the markdown file."""
-        with open(f'{self.file_name}', 'r+', encoding='utf-8') as self.file:
+        :param str data: is a string containing all the data that is written in the markdown file.
+        """
+        with open(f"{self.file_name}", "r+", encoding="utf-8") as self.file:
             file_data = self.file.read()  # Save all the file's content
             self.file.seek(0, 0)  # Place file pointer at the beginning
             first_line = self.file.readline()  # Read the first line
             second_line = self.file.readline()  # Read the second line
-            self.file.seek(len(first_line + second_line), 0)  # Place file pointer at the end of the first line
+            self.file.seek(
+                len(first_line + second_line), 0
+            )  # Place file pointer at the end of the first line
             self.file.write(data)  # Write data
-            self.file.write('\n' + file_data[len(first_line + second_line):])
+            self.file.write("\n" + file_data[len(first_line + second_line):])
 
     @staticmethod
     def read_file(file_name: str) -> str:
         """Read a Markdown file using a file name. It is not necessary to add *.md extension.
 
         :param file_name: Markdown file's name.
         :type file_name: str
         :return: return all file's data.
         :rtype: str"""
 
-        if file_name.find('.md') == -1:
-            file_name += '.md'
+        if file_name.find(".md") == -1:
+            file_name += ".md"
 
-        with open(file_name, 'r', encoding='utf-8') as file:
+        with open(file_name, "r", encoding="utf-8") as file:
             file_data = file.read()
 
         return file_data
 
 
-if __name__ == '__main__':
-    new_file = MarkDownFile('Example')
+if __name__ == "__main__":
+    new_file = MarkDownFile("Example")
     new_file.rewrite_all_file(data="# Some Text Example")
```

### Comparing `mdutils-1.5.1/mdutils/mdutils.py` & `mdutils-1.6.0/mdutils/mdutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from mdutils.fileutils.fileutils import MarkDownFile
 from mdutils.tools.Header import Header
 from mdutils.tools.Image import Image
 from mdutils.tools.Link import Inline, Reference
 from mdutils.tools.TextUtils import TextUtils
 from mdutils.tools.MDList import MDList, MDCheckbox
 from textwrap import fill
+from typing import Union, Optional, List
 
 
 class MdUtils:
     """This class give some basic methods that helps the creation of Markdown files while you are executing a python
     code.
 
     The ``__init__`` variables are:
@@ -40,64 +41,79 @@
     - **header:** it is an instance of Header Class.
     - **textUtils:** it is an instance of TextUtils Class.
     - **title:** it is the title of the Markdown file. It is written with Setext-style.
     - **table_of_contents:** it is the table of contents, it can be optionally created.
     - **file_data_text:** contains all the file data that will be written on the markdown file.
     """
 
-    def __init__(self, file_name, title="", author=""):
+    def __init__(self, file_name: str, title: str = "", author: str = ""):
         """
 
         :param file_name: it is the name of the Markdown file.
         :type file_name: str
         :param title: it is the title of the Markdown file. It is written with Setext-style.
         :type title: str
         :param author: it is the author fo the Markdown file.
         :type author: str
         """
         self.file_name = file_name
         self.author = author
         self.header = Header()
         self.textUtils = TextUtils
-        self.title = self.header.choose_header(level=1, title=title, style='setext')
+        self.title = self.header.choose_header(level=1, title=title, style="setext")
         self.table_of_contents = ""
         self.file_data_text = ""
         self._table_titles = []
         self.reference = Reference()
         self.image = Image(reference=self.reference)
 
-    def create_md_file(self):
+    def create_md_file(self) -> MarkDownFile:
         """It creates a new Markdown file.
         :return: return an instance of a MarkDownFile."""
         md_file = MarkDownFile(self.file_name)
         md_file.rewrite_all_file(
-            data=self.title + self.table_of_contents + self.file_data_text + self.reference.get_references_as_markdown()
+            data=self.title
+            + self.table_of_contents
+            + self.file_data_text
+            + self.reference.get_references_as_markdown()
         )
         return md_file
 
     def get_md_text(self) -> str:
         """Instead of writing the markdown text into a file it returns it as a string.
 
         :return: return a string with the markdown text."""
-        return self.title + self.table_of_contents + self.file_data_text + self.reference.get_references_as_markdown()
+        return (
+            self.title
+            + self.table_of_contents
+            + self.file_data_text
+            + self.reference.get_references_as_markdown()
+        )
 
-    def read_md_file(self, file_name):
+    def read_md_file(self, file_name: str) -> str:
         """Reads a Markdown file and save it to global class `file_data_text`.
 
         :param file_name: Markdown file's name that has to be read.
         :type file_name: str
         :return: optionally returns the file data content.
         :rtype: str
         """
         file_data = MarkDownFile().read_file(file_name)
         self.___update_file_data(file_data)
 
         return file_data
 
-    def new_header(self, level, title, style='atx', add_table_of_contents='y', header_id=''):
+    def new_header(
+        self,
+        level: int,
+        title: str,
+        style: str = "atx",
+        add_table_of_contents: str = "y",
+        header_id: str = "",
+    ) -> str:
         """Add a new header to the Markdown file.
 
         :param level: Header level. *atx* style can take values 1 til 6 and *setext* style take values 1 and 2.
         :type level: int
         :param title: Header title.
         :type title: str
         :param style: Header style, can be ``'atx'`` or ``'setext'``. By default ``'atx'`` style is chosen.
@@ -113,41 +129,44 @@
         >>> mdfile = MdUtils("Header_Example")
         >>> print(mdfile.new_header(level=2, title='Header Level 2 Title', style='atx', add_table_of_contents='y'))
         '\\n## Header Level 2 Title\\n'
         >>> print(mdfile.new_header(level=2, title='Header Title', style='setext'))
         '\\nHeader Title\\n-------------\\n'
 
         """
-        if add_table_of_contents == 'y':
+        if add_table_of_contents == "y":
             self.__add_new_item_table_of_content(level, title)
-        self.___update_file_data(self.header.choose_header(level, title, style, header_id))
+        self.___update_file_data(
+            self.header.choose_header(level, title, style, header_id)
+        )
         return self.header.choose_header(level, title, style, header_id)
 
-    def __add_new_item_table_of_content(self, level, item):
+    def __add_new_item_table_of_content(self, level: int, item: Union[List[str], str]):
         """Automatically add new atx headers to the table of contents.
 
         :param level: add levels up to 6.
         :type level: int
         :param item: items to add.
         :type item: list or str
 
         """
 
         curr = self._table_titles
 
-        for i in range(level-1):
+        for i in range(level - 1):
             curr = curr[-1]
 
         curr.append(item)
 
         if level < 6:
             curr.append([])
 
-
-    def new_table_of_contents(self, table_title="Table of contents", depth=1, marker=''):
+    def new_table_of_contents(
+        self, table_title: str = "Table of contents", depth: int = 1, marker: str = ""
+    ) -> str:
         """Table of contents can be created if Headers of 'atx' style have been defined.
 
         This method allows to create a table of contents and define a title for it. Moreover, `depth` allows user to
         define how many levels of headers will be placed in the table of contents.
         If no marker is defined, the table of contents will be placed automatically after the file's title.
 
         :param table_title: The table content's title, by default "Table of contents"
@@ -159,27 +178,42 @@
         :return: a string with the data is returned.
         :rtype: str
 
         """
 
         if marker:
             self.table_of_contents = ""
-            marker_table_of_contents = self.header.choose_header(level=1, title=table_title, style='setext')
+            marker_table_of_contents = self.header.choose_header(
+                level=1, title=table_title, style="setext"
+            )
             marker_table_of_contents += mdutils.tools.TableOfContents.TableOfContents().create_table_of_contents(
-                self._table_titles, depth)
-            self.file_data_text = self.place_text_using_marker(marker_table_of_contents, marker)
+                self._table_titles, depth
+            )
+            self.file_data_text = self.place_text_using_marker(
+                marker_table_of_contents, marker
+            )
         else:
             marker_table_of_contents = ""
-            self.table_of_contents += self.header.choose_header(level=1, title=table_title, style='setext')
+            self.table_of_contents += self.header.choose_header(
+                level=1, title=table_title, style="setext"
+            )
             self.table_of_contents += mdutils.tools.TableOfContents.TableOfContents().create_table_of_contents(
-                self._table_titles, depth)
+                self._table_titles, depth
+            )
 
         return self.table_of_contents + marker_table_of_contents
 
-    def new_table(self, columns, rows, text, text_align='center', marker=''):
+    def new_table(
+        self,
+        columns: int,
+        rows: int,
+        text: List[str],
+        text_align: str = "center",
+        marker: str = "",
+    ) -> str:
         """This method takes a list of strings and creates a table.
 
             Using arguments ``columns`` and ``rows`` allows to create a table of *n* columns and *m* rows. The
             ``columns * rows`` operations has to correspond to the number of elements of ``text`` list argument.
             Moreover, ``argument`` allows to place the table wherever you want from the file.
 
         :param columns: this variable defines how many columns will have the table.
@@ -218,138 +252,184 @@
         if marker:
             self.file_data_text = self.place_text_using_marker(text_table, marker)
         else:
             self.___update_file_data(text_table)
 
         return text_table
 
-    def new_paragraph(self, text='', bold_italics_code='', color='black', align='', wrap_width=0):
+    def new_paragraph(
+        self,
+        text: str = "",
+        bold_italics_code: str = "",
+        color: str = "black",
+        align: str = "",
+        wrap_width: int = 0,
+    ) -> str:
         """Add a new paragraph to Markdown file. The text is saved to the global variable file_data_text.
 
         :param text: is a string containing the paragraph text. Optionally, the paragraph text is returned.
         :type text: str
         :param bold_italics_code: using ``'b'``: **bold**, ``'i'``: *italics* and ``'c'``: ``inline_code``.
         :type bold_italics_code: str
         :param color: Can change text color. For example: ``'red'``, ``'green'``, ``'orange'``...
         :type color: str
         :param align: Using this parameter you can align text.
         :type align: str
-        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not broken. 
-                           Use width of 0 to disable wrapping.
+        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not
+                           broken. Use width of 0 to disable wrapping.
         :type wrap_width: int
         :return:  ``'\\n\\n' + text``. Not necessary to take it, if only has to be written to
                     the file.
         :rtype: str
 
         """
 
         if wrap_width > 0:
-            text = fill(text, wrap_width, break_long_words=False, replace_whitespace=False, drop_whitespace=False)
-
-        if bold_italics_code or color != 'black' or align:
-            self.___update_file_data('\n\n' + self.textUtils.text_format(text, bold_italics_code, color, align))
+            text = fill(
+                text,
+                wrap_width,
+                break_long_words=False,
+                replace_whitespace=False,
+                drop_whitespace=False,
+            )
+
+        if bold_italics_code or color != "black" or align:
+            self.___update_file_data(
+                "\n\n"
+                + self.textUtils.text_format(text, bold_italics_code, color, align)
+            )
         else:
-            self.___update_file_data('\n\n' + text)
+            self.___update_file_data("\n\n" + text)
 
         return self.file_data_text
 
-    def new_line(self, text='', bold_italics_code='', color='black', align='', wrap_width=0):
+    def new_line(
+        self,
+        text: str = "",
+        bold_italics_code: str = "",
+        color: str = "black",
+        align: str = "",
+        wrap_width: int = 0,
+    ) -> str:
         """Add a new line to Markdown file. The text is saved to the global variable file_data_text.
 
         :param text: is a string containing the paragraph text. Optionally, the paragraph text is returned.
         :type text: str
         :param bold_italics_code: using ``'b'``: **bold**, ``'i'``: *italics* and ``'c'``: ``inline_code``...
         :type bold_italics_code: str
         :param color: Can change text color. For example: ``'red'``, ``'green'``, ``'orange'``...
         :type color: str
         :param align: Using this parameter you can align text. For example ``'right'``, ``'left'`` or ``'center'``.
         :type align: str
-        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not broken. 
-                           Use width of 0 to disable wrapping.
+        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not
+                           broken. Use width of 0 to disable wrapping.
         :type wrap_width: int
         :return: return a string ``'\\n' + text``. Not necessary to take it, if only has to be written to the
                     file.
         :rtype: str
         """
 
         if wrap_width > 0:
-            text = fill(text, wrap_width, break_long_words=False, replace_whitespace=False, drop_whitespace=False)
-
-        if bold_italics_code or color != 'black' or align:
-            self.___update_file_data('  \n' + self.textUtils.text_format(text, bold_italics_code, color, align))
+            text = fill(
+                text,
+                wrap_width,
+                break_long_words=False,
+                replace_whitespace=False,
+                drop_whitespace=False,
+            )
+
+        if bold_italics_code or color != "black" or align:
+            self.___update_file_data(
+                "  \n"
+                + self.textUtils.text_format(text, bold_italics_code, color, align)
+            )
         else:
-            self.___update_file_data('  \n' + text)
+            self.___update_file_data("  \n" + text)
 
         return self.file_data_text
 
-    def write(self, text='', bold_italics_code='', color='black', align='', marker='', wrap_width=0):
+    def write(
+        self,
+        text: str = "",
+        bold_italics_code: str = "",
+        color: str = "black",
+        align: str = "",
+        marker: str = "",
+        wrap_width: int = 0,
+    ) -> str:
         """Write text in ``file_Data_text`` string.
 
         :param text: a text a string.
         :type text: str
         :param bold_italics_code: using ``'b'``: **bold**, ``'i'``: *italics* and ``'c'``: ``inline_code``...
         :type bold_italics_code: str
         :param color: Can change text color. For example: ``'red'``, ``'green'``, ``'orange'``...
         :type color: str
         :param align: Using this parameter you can align text. For example ``'right'``, ``'left'`` or ``'center'``.
         :type align: str
-        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not broken. 
-                           Use width of 0 to disable wrapping.
+        :param wrap_width: wraps text with designated width by number of characters. By default, long words are not
+                           broken. Use width of 0 to disable wrapping.
         :type wrap_width: int
         :param marker: allows to replace a marker on some point of the file by the text.
         :type marker: str
         """
 
         if wrap_width > 0:
-            text = fill(text, wrap_width, break_long_words=False, replace_whitespace=False, drop_whitespace=False)
+            text = fill(
+                text,
+                wrap_width,
+                break_long_words=False,
+                replace_whitespace=False,
+                drop_whitespace=False,
+            )
 
         if bold_italics_code or color or align:
             new_text = self.textUtils.text_format(text, bold_italics_code, color, align)
         else:
             new_text = text
 
         if marker:
             self.file_data_text = self.place_text_using_marker(new_text, marker)
         else:
             self.___update_file_data(new_text)
 
         return new_text
 
-    def insert_code(self, code, language=''):
+    def insert_code(self, code: str, language: str = "") -> str:
         """This method allows to insert a peace of code on a markdown file.
 
         :param code: code string.
         :type code: str
         :param language: code language: python, c++, c#...
         :type language: str
         :return:
         :rtype: str
         """
-        md_code = '\n\n' + self.textUtils.insert_code(code, language)
+        md_code = "\n\n" + self.textUtils.insert_code(code, language)
         self.___update_file_data(md_code)
         return md_code
 
-    def create_marker(self, text_marker):
+    def create_marker(self, text_marker: str) -> str:
         """This will add a marker to ``file_data_text`` and returns the marker result in order to be used whenever
             you need.
 
             Markers allows to place them to the string data text and they can be replaced by a peace of text using
             ``place_text_using_marker`` method.
 
         :param text_marker: marker name.
         :type text_marker: str
         :return: return a marker of the following form: ``'##--[' + text_marker + ']--##'``
         :rtype: str
         """
 
-        new_marker = '##--[' + text_marker + ']--##'
+        new_marker = "##--[" + text_marker + "]--##"
         self.___update_file_data(new_marker)
         return new_marker
 
-    def place_text_using_marker(self, text, marker):
+    def place_text_using_marker(self, text: str, marker: str) -> str:
         """It replace a previous marker created with ``create_marker`` with a text string.
 
             This method is going to search for the ``marker`` argument, which has been created previously using
             ``create_marker`` method, in ``file_data_text`` string.
 
         :param text: the new string that will replace the marker.
         :type text: str
@@ -359,15 +439,21 @@
         :rtype: str
         """
         return self.file_data_text.replace(marker, text)
 
     def ___update_file_data(self, file_data):
         self.file_data_text += file_data
 
-    def new_inline_link(self, link, text=None, bold_italics_code='', align=''):
+    def new_inline_link(
+        self,
+        link: str,
+        text: Optional[str] = None,
+        bold_italics_code: str = "",
+        align: str = "",
+    ) -> str:
         """Creates a inline link in markdown format.
 
         :param link:
         :type link: str
         :param text: Text that is going to be displayed in the markdown file as a link.
         :type text: str
         :param bold_italics_code: Using ``'b'``: **bold**, ``'i'``: *italics* and ``'c'``: ``inline_code``...
@@ -384,19 +470,28 @@
         """
         if text is None:
             n_text = link
         else:
             n_text = text
 
         if bold_italics_code or align:
-            n_text = self.textUtils.text_format(text=n_text, bold_italics_code=bold_italics_code, align=align)
+            n_text = self.textUtils.text_format(
+                text=n_text, bold_italics_code=bold_italics_code, align=align
+            )
 
         return Inline.new_link(link=link, text=n_text)
 
-    def new_reference_link(self, link, text, reference_tag=None, bold_italics_code='', align=''):
+    def new_reference_link(
+        self,
+        link: str,
+        text: str,
+        reference_tag: Optional[str] = None,
+        bold_italics_code: str = "",
+        align: str = "",
+    ) -> str:
         """Creates a reference link in markdown format. All references will be stored at the end of the markdown file.
 
 
         :param link:
         :type link: str
         :param text: Text that is going to be displayed in the markdown file as a link.
         :type text: str
@@ -428,41 +523,49 @@
         >>> print(repr(link))
         '[**mdutils**][md]'
         >>> md.create_md_file()
 
         """
 
         if reference_tag is None:
-            if bold_italics_code != '':
-                raise TypeError('For using bold_italics_code param, reference_tag must be defined')
-            if align != '':
-                raise TypeError('For using align, reference_tag must be defined')
+            if bold_italics_code != "":
+                raise TypeError(
+                    "For using bold_italics_code param, reference_tag must be defined"
+                )
+            if align != "":
+                raise TypeError("For using align, reference_tag must be defined")
 
         n_text = text
         if bold_italics_code or align:
-            n_text = self.textUtils.text_format(text=n_text, bold_italics_code=bold_italics_code, align=align)
+            n_text = self.textUtils.text_format(
+                text=n_text, bold_italics_code=bold_italics_code, align=align
+            )
 
-        return self.reference.new_link(link=link, text=n_text, reference_tag=reference_tag)
+        return self.reference.new_link(
+            link=link, text=n_text, reference_tag=reference_tag
+        )
 
     @staticmethod
-    def new_inline_image(text, path):
+    def new_inline_image(text: str, path: str) -> str:
         """Add inline images in a markdown file. For example ``[MyImage](../MyImage.jpg)``.
 
         :param text: Text that is going to be displayed in the markdown file as a iamge.
         :type text: str
         :param path: Image's path / link.
         :type path: str
         :return: return the image in markdown format ``'![ + text + '](' + path + ')'``.
         :rtype: str
 
         """
 
         return Image.new_inline_image(text=text, path=path)
 
-    def new_reference_image(self, text, path, reference_tag=None):
+    def new_reference_image(
+        self, text: str, path: str, reference_tag: Optional[str] = None
+    ) -> str:
         """Add reference images in a markdown file. For example ``[MyImage][my_image]``. All references will be stored
         at the end of the markdown file.
 
         :param text: Text that is going to be displayed in the markdown file as a image.
         :type text: str
         :param path: Image's path / link.
         :type path: str
@@ -470,40 +573,42 @@
         :type reference_tag: str
         :return: return the image in markdown format ``'![ + text + '][' + reference_tag + ']'``.
         :rtype: str
 
         .. note::
             If param reference_tag is not provided, text param will be used instead.
         """
-        return self.image.new_reference_image(text=text, path=path, reference_tag=reference_tag)
+        return self.image.new_reference_image(
+            text=text, path=path, reference_tag=reference_tag
+        )
 
-    def new_list(self, items: [str], marked_with: str = "-"):
+    def new_list(self, items: List[str], marked_with: str = "-"):
         """Add unordered or ordered list in MarkDown file.
 
         :param items: Array of items for generating the list.
         :type items: [str]
         :param marked_with: By default has the value of ``'-'``, can be ``'+'``, ``'*'``. If you want to generate
          an ordered list then set to ``'1'``.
         :type marked_with: str
         :return:
         """
         mdlist = MDList(items, marked_with)
-        self.___update_file_data('\n' + mdlist.get_md())
+        self.___update_file_data("\n" + mdlist.get_md())
 
-    def new_checkbox_list(self, items: [str], checked: bool = False):
+    def new_checkbox_list(self, items: List[str], checked: bool = False):
         """Add checkbox list in MarkDown file.
 
         :param items: Array of items for generating the checkbox list.
         :type items: [str]
         :param checked: if you set this to ``True``. All checkbox will be checked. By default is ``False``.
         :type checked: bool
         :return:
         """
 
         mdcheckbox = MDCheckbox(items=items, checked=checked)
-        self.___update_file_data('\n' + mdcheckbox.get_md())
+        self.___update_file_data("\n" + mdcheckbox.get_md())
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `mdutils-1.5.1/mdutils/tools/Header.py` & `mdutils-1.6.0/mdutils/tools/Header.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,124 +21,124 @@
     * Add color to text.
     """
 
     # ********************************************************************
     # *                             Atx-Style                            *
     # ********************************************************************
     @staticmethod
-    def atx_level_1(title, header_id=''):
+    def atx_level_1(title: str, header_id: str = "") -> str:
         """Return a atx level 1 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n#' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n# ' + title + header_id + '\n'
+        return "\n# " + title + header_id + "\n"
 
     @staticmethod
-    def atx_level_2(title, header_id=''):
+    def atx_level_2(title: str, header_id: str = "") -> str:
         """Return a atx level 2 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n##' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n## ' + title + header_id + '\n'
+        return "\n## " + title + header_id + "\n"
 
     @staticmethod
-    def atx_level_3(title, header_id=''):
+    def atx_level_3(title: str, header_id: str = "") -> str:
         """Return a atx level 3 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n###' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n### ' + title + header_id + '\n'
+        return "\n### " + title + header_id + "\n"
 
     @staticmethod
-    def atx_level_4(title, header_id=''):
+    def atx_level_4(title: str, header_id: str = "") -> str:
         """Return a atx level 4 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n####' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n#### ' + title + header_id + '\n'
+        return "\n#### " + title + header_id + "\n"
 
     @staticmethod
-    def atx_level_5(title, header_id=''):
+    def atx_level_5(title: str, header_id: str = "") -> str:
         """Return a atx level 5 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n#####' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n##### ' + title + header_id + '\n'
+        return "\n##### " + title + header_id + "\n"
 
     @staticmethod
-    def atx_level_6(title, header_id=''):
+    def atx_level_6(title: str, header_id: str = "") -> str:
         """Return a atx level 6 header.
 
         :param str title: text title.
         :param header_id: ID of the header for extended Markdown syntax
         :return: a header title of form: ``'\\n######' + title + '\\n'``
         :rtype: str
         """
         if len(header_id):
-            header_id = ' {#' + header_id + '}'
+            header_id = " {#" + header_id + "}"
 
-        return '\n###### ' + title + header_id + '\n'
+        return "\n###### " + title + header_id + "\n"
 
     # ********************************************************************
     # *                          Setext-Style                            *
     # ********************************************************************
     @staticmethod
-    def setext_level_1(title):
+    def setext_level_1(title: str) -> str:
         """Return a setext level 1 header.
 
         :param str title: text title.
         :return: a header titlte of form: ``'\\n' + title +'\\n==========\\n'``.
         :rtype: str
         """
 
-        return '\n' + title + '\n' + ''.join(['=' for _ in title]) + '\n'
+        return "\n" + title + "\n" + "".join(["=" for _ in title]) + "\n"
 
     @staticmethod
-    def setext_level_2(title):
+    def setext_level_2(title: str) -> str:
         """Return a setext level 1 header.
 
-                :param str title: text title.
-                :return: a header titlte of form: ``'\\n' + title +'\\n------------\\n'``.
-                :rtype: str
+        :param str title: text title.
+        :return: a header titlte of form: ``'\\n' + title +'\\n------------\\n'``.
+        :rtype: str
         """
 
-        return '\n' + title + '\n' + ''.join(['-' for _ in title]) + '\n'
+        return "\n" + title + "\n" + "".join(["-" for _ in title]) + "\n"
 
     @staticmethod
-    def header_anchor(text, link=""):
+    def header_anchor(text: str, link: str = "") -> str:
         """Creates an internal link of a defined Header level 1 or level 2 in the markdown file.
 
         Giving a text string an text link you can create an internal link of already existing header. If the ``link``
         string does not contain '#', it will creates an automatic link of the type ``#title-1``.
 
         :param text: it is the text that will be displayed.
         :param link: it is the internal link.
@@ -146,67 +146,76 @@
         :type text: str
         :type link: str
         :rtype: string
 
         **Example:** [Title 1](#title-1)
         """
         if link:
-            if link[0] != '#':
-                link = link.lower().replace(' ', '-')
+            if link[0] != "#":
+                link = link.lower().replace(" ", "-")
             else:
-                link = '#' + link
+                link = "#" + link
         else:
-            link = '#' + text.lower().replace(' ', '-')
+            link = "#" + text.lower().replace(" ", "-")
 
-        return '[' + text + '](' + link + ')'
+        return "[" + text + "](" + link + ")"
 
     @staticmethod
-    def choose_header(level, title, style='atx', header_id=''):
+    def choose_header(
+        level: int, title: str, style: str = "atx", header_id: str = ""
+    ) -> str:
         # noinspection SpellCheckingInspection
         """This method choose the style and the header level.
 
-                    :Examples:
-                    >>> from mdutils.tools.Header import Header
-                    >>> Header.choose_header(level=1, title='New Header', style='atx')
-                    '\\n# New Header\\n'
-
-                    >>> Header.choose_header(level=2, title='Another Header 1', style='setext')
-                    '\\nAnother Header 1\\n----------------\\n'
-
-                :param level: Header Level, For Atx-style 1 til 6. For Setext-style 1 and 2 header levels.
-                :param title: Header Title.
-                :param style: Header Style atx or setext.
-                :param header_id: ID of the header for extended Markdown syntax
-                :return:
-                """
-        if style.lower() == 'atx':
+            :Examples:
+            >>> from mdutils.tools.Header import Header
+            >>> Header.choose_header(level=1, title='New Header', style='atx')
+            '\\n# New Header\\n'
+
+            >>> Header.choose_header(level=2, title='Another Header 1', style='setext')
+            '\\nAnother Header 1\\n----------------\\n'
+
+        :param level: Header Level, For Atx-style 1 til 6. For Setext-style 1 and 2 header levels.
+        :param title: Header Title.
+        :param style: Header Style atx or setext.
+        :param header_id: ID of the header for extended Markdown syntax
+        :return:
+        """
+        if style.lower() == "atx":
             if level == 1:
                 return Header.atx_level_1(title, header_id)
             elif level == 2:
                 return Header.atx_level_2(title, header_id)
             elif level == 3:
                 return Header.atx_level_3(title, header_id)
             elif level == 4:
                 return Header.atx_level_4(title, header_id)
             elif level == 5:
                 return Header.atx_level_5(title, header_id)
             elif level == 6:
                 return Header.atx_level_6(title, header_id)
             else:
-                raise ValueError("For 'atx' style, level's expected value: 1, 2, 3, 4, 5 or 6, but level = "
-                                 + str(level))
-        elif style.lower() == 'setext':
+                raise ValueError(
+                    "For 'atx' style, level's expected value: 1, 2, 3, 4, 5 or 6, but level = "
+                    + str(level)
+                )
+        elif style.lower() == "setext":
             if level == 1:
                 return Header.setext_level_1(title)
             elif level == 2:
                 return Header.setext_level_2(title)
             else:
-                raise ValueError("For 'setext' style, level's expected value: 1, 2, 3, 4, 5 or 6, but level = "
-                                 + str(level))
+                raise ValueError(
+                    "For 'setext' style, level's expected value: 1, 2, 3, 4, 5 or 6, but level = "
+                    + str(level)
+                )
         else:
-            raise ValueError("style's expected value: 'atx' or 'setext', but style = " + style.lower())
+            raise ValueError(
+                "style's expected value: 'atx' or 'setext', but style = "
+                + style.lower()
+            )
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `mdutils-1.5.1/mdutils/tools/Html.py` & `mdutils-1.6.0/mdutils/tools/Html.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 #
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2020 Dídac Coll
 
 
 class Html:
-
     @staticmethod
     def paragraph(text: str, align: str = None) -> str:
         """
         :param text:
         :param align: ``center`` or ``right``.
         :type align: str
         :return: ``"<p align=\"{}\">\\n    {}\\n</p>".format(align, text)``.
         :rtype: str
         """
 
         if align is None:
-            return '<p>\n    {}\n</p>'.format(text)
+            return "<p>\n    {}\n</p>".format(text)
 
         if align is not None:
             if align not in ["left", "center", "right"]:
                 raise KeyError
 
         return '<p align="{}">\n    {}\n</p>'.format(align, text)
 
@@ -45,44 +44,50 @@
         :Example:
         >>> Html.image(path='../image.jpg', size='200', align='center')
         >>> Html.image(path='../image.jpg', size='x200', align='left')
         >>> Html.image(path='../image.jpg', size='300x400')
         """
 
         if align:
-            return cls.paragraph(text=cls.__html_image(path=path, size=size), align=align)
+            return cls.paragraph(
+                text=cls.__html_image(path=path, size=size), align=align
+            )
 
         return cls.__html_image(path=path, size=size)
 
     @classmethod
     def __html_image(cls, path: str, size: str = None):
         if size:
-            return '<img src="{}" {}/>'.format(path, HtmlSize.size_to_width_and_height(size=size))
+            return '<img src="{}" {}/>'.format(
+                path, HtmlSize.size_to_width_and_height(size=size)
+            )
         return '<img src="{}" />'.format(path)
 
 
 class HtmlSize:
     @classmethod
     def size_to_width_and_height(cls, size: str) -> str:
         size = cls.__pre_process_size(size=size)
         if size.isdigit():
             return cls.__get_width(size=size)
 
-        if size.startswith('x'):
+        if size.startswith("x"):
             height = size[1:]
             if height.isdigit():
                 return cls.__get_height(size=height)
 
             raise SizeBadFormat(size)
 
-        width_height = size.split('x')
+        width_height = size.split("x")
 
         if len(width_height) == 2:
             if width_height[0].isdigit() and width_height[1].isdigit():
-                return "{} {}".format(cls.__get_width(width_height[0]), cls.__get_height(width_height[1]))
+                return "{} {}".format(
+                    cls.__get_width(width_height[0]), cls.__get_height(width_height[1])
+                )
 
         raise SizeBadFormat(size)
 
     @classmethod
     def __pre_process_size(cls, size: str) -> str:
         no_spaces = size.replace(" ", "")
         return no_spaces.lower()
@@ -94,10 +99,17 @@
     @classmethod
     def __get_height(cls, size: str):
         return 'height="{}"'.format(int(size))
 
 
 class SizeBadFormat(Exception):
     """Raise exception when size does not match the expected format"""
+
     def __init__(self, message):
-        Exception.__init__(self, "Unexpected format: {}. Expected: '<int>', 'x<int>' or '<int>x<int>'".format(message))
+        Exception.__init__(
+            self,
+            "Unexpected format: {}. Expected: '<int>', 'x<int>' or '<int>x<int>'".format(
+                message
+            ),
+        )
+
     pass
```

### Comparing `mdutils-1.5.1/mdutils/tools/Image.py` & `mdutils-1.6.0/mdutils/tools/Image.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,52 @@
 #
 # MIT License: (C) 2020 Dídac Coll
 
 from mdutils.tools.Link import Inline, Reference
 
 
 class Image:
-
-    def __init__(self, reference):
+    def __init__(self, reference: Reference):
         """
         :param reference:
         :type reference: Reference
         """
         self.reference = reference
 
     @staticmethod
-    def new_inline_image(text, path, tooltip=None):
+    def new_inline_image(text: str, path: str, tooltip: str = None) -> str:
         """
         :param text: Text that is going to be displayed in the markdown file as a iamge.
         :type text: str
         :param path: Image's path / link.
         :type path: str
         :param tooltip:
         :type tooltip: str
         :return: return the image in markdown format ``'![ + text + '](' + path + 'tooltip' + ')'``.
         :rtype: str
         """
-        return '!' + Inline.new_link(link=path, text=text, tooltip=tooltip)
+        return "!" + Inline.new_link(link=path, text=text, tooltip=tooltip)
 
-    def new_reference_image(self, text, path, reference_tag=None, tooltip=None):
+    def new_reference_image(
+        self, text: str, path: str, reference_tag: str = None, tooltip: str = None
+    ) -> str:
         """
         :param text: Text that is going to be displayed in the markdown file as a image.
         :type text: str
         :param path: Image's path / link.
         :type path: str
         :param reference_tag: Tag that will be placed at the end of the markdown file jointly with the image's path.
         :type reference_tag: str
         :param tooltip:
         :type tooltip: str
         :return: return the image in markdown format ``'![ + text + '][' + reference_tag + ']'``.
         :rtype: str
         """
-        return '!' + self.reference.new_link(link=path, text=text, reference_tag=reference_tag, tooltip=tooltip)
+        return "!" + self.reference.new_link(
+            link=path, text=text, reference_tag=reference_tag, tooltip=tooltip
+        )
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `mdutils-1.5.1/mdutils/tools/Link.py` & `mdutils-1.6.0/mdutils/tools/Link.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,95 +5,101 @@
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2020 Dídac Coll
 from mdutils.tools.TextUtils import TextUtils
 
 
 class Reference:
-
     def __init__(self):
         self.references = {}
 
-    def get_references(self):
+    def get_references(self) -> dict:
         """
         :return:
         :rtype: dict
         """
         return self.references
 
-    def get_references_as_markdown(self):
+    def get_references_as_markdown(self) -> str:
         """
         :return:
         :rtype: str
         """
         if not bool(self.references):
             return ""
 
         references_as_markdown = ""
         for key in sorted(self.references.keys()):
-            references_as_markdown += '[' + key + ']: ' + self.references[key] + '\n'
-        return '\n\n\n' + references_as_markdown
+            references_as_markdown += "[" + key + "]: " + self.references[key] + "\n"
+        return "\n\n\n" + references_as_markdown
 
-    def new_link(self, link, text, reference_tag=None, tooltip=None):
+    def new_link(
+        self, link: str, text: str, reference_tag: str = None, tooltip: str = None
+    ) -> str:
         """
         :param link:
         :type link: str
         :param text: Text that is going to be displayed in the markdown file as a link.
         :type text: str
         :param reference_tag: Reference that will be saved on reference dict.
         :type reference_tag: str
         :param tooltip: Add a tooltip on the link.
         :type tooltip: str
         :return: ``'[' + text + '][' + reference_tag + ']'`` or if reference_Tag is not defined: ``'[' + text + ']'``.
         :rtype: str
         """
         if reference_tag is None:
             self.__update_ref(link, text, tooltip)
-            return '[' + text + ']'
+            return "[" + text + "]"
 
         self.__update_ref(link, reference_tag, tooltip)
-        return '[' + text + '][' + reference_tag + ']'
+        return "[" + text + "][" + reference_tag + "]"
 
-    def __update_ref(self, link, reference_tag, tooltip=None):
+    def __update_ref(self, link: str, reference_tag: str, tooltip: str = None):
         if not (reference_tag in self.references.keys()):
             if tooltip is not None:
-                self.references.update({reference_tag: TextUtils.add_tooltip(link, tooltip)})
+                self.references.update(
+                    {reference_tag: TextUtils.add_tooltip(link, tooltip)}
+                )
                 return
 
             self.references.update({reference_tag: link})
 
 
 class Inline:
-
     @staticmethod
-    def new_link(link, text=None, tooltip=None):
+    def new_link(link: str, text: str = None, tooltip: str = None):
         """
         :param link:
         :type link: str
         :param text: Text that is going to be displayed in the markdown file as a link.
         :type text: str
         :param tooltip: Add a tool tip on the image.
         :type tooltip: str
         :return: ``'[' + text +'](' + link + 'tooltip' + ')'`` or if link is only defined: ```<` + link '>'``.
         :rtype: str
         """
 
         if tooltip:
             if text is None:
-                return Inline.__md_link(link=TextUtils.add_tooltip(link=link, tip=tooltip), text=link)
-
-            return Inline.__md_link(link=TextUtils.add_tooltip(link=link, tip=tooltip), text=text)
+                return Inline.__md_link(
+                    link=TextUtils.add_tooltip(link=link, tip=tooltip), text=link
+                )
+
+            return Inline.__md_link(
+                link=TextUtils.add_tooltip(link=link, tip=tooltip), text=text
+            )
 
         if text is None:
-            return '<' + link + '>'
+            return "<" + link + ">"
 
         return Inline.__md_link(link=link, text=text)
 
     @staticmethod
-    def __md_link(link, text):
+    def __md_link(link: str, text: str):
         return TextUtils.text_external_link(text, link)
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `mdutils-1.5.1/mdutils/tools/MDList.py` & `mdutils-1.6.0/mdutils/tools/MDList.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,105 +8,119 @@
 import re
 
 
 class MDListHelper:
     def __init__(self):
         self.n_tabs = 0
 
-    def _get_unordered_markdown_list(self, items: [str], marker: str) -> str:
+    def _get_unordered_markdown_list(self, items, marker: str) -> str:
         md_list = ""
         for item in items:
             if isinstance(item, list):
                 self.n_tabs += 1
                 md_list += self._get_unordered_markdown_list(item, marker)
                 self.n_tabs -= 1
             else:
                 md_list += self._add_new_item(item, marker)
 
         return md_list
 
-    def _get_ordered_markdown_list(self, items: [str]) -> str:
+    def _get_ordered_markdown_list(self, items) -> str:
         md_list = ""
         n_marker = 1
         for item in items:
             if isinstance(item, list):
                 self.n_tabs += 1
                 md_list += self._get_ordered_markdown_list(items=item)
                 self.n_tabs -= 1
             else:
                 md_list += self._add_new_item(item, f"{n_marker}.")
                 n_marker += 1
         return md_list
 
     def _add_new_item(self, item: str, marker: str):
-        item_with_hyphen = item if self._is_there_marker_in_item(item) else self._add_hyphen(item, marker)
-        return self._n_spaces(4 * self.n_tabs) + item_with_hyphen + '\n'
+        item_with_hyphen = (
+            item
+            if self._is_there_marker_in_item(item)
+            else self._add_hyphen(item, marker)
+        )
+        return self._n_spaces(4 * self.n_tabs) + item_with_hyphen + "\n"
 
     @classmethod
     def _is_there_marker_in_item(cls, item: str) -> bool:
-        if item.startswith('-') or item.startswith('*') or item.startswith('+') or re.search(r"^(\d\.)", item):
+        if (
+            item.startswith("-")
+            or item.startswith("*")
+            or item.startswith("+")
+            or re.search(r"^(\d\.)", item)
+        ):
             return True
         return False
 
     @classmethod
     def _add_hyphen(cls, item: str, marker: str):
         return f"{marker} {item}"
 
     @classmethod
     def _n_spaces(cls, number_spaces: int = 1):
         return " " * number_spaces
 
 
 class MDList(MDListHelper):
-    """This class allows to create unordered or ordered MarkDown list.
+    """This class allows to create unordered or ordered MarkDown list."""
 
-    """
-    def __init__(self, items: [str], marked_with: str = '-'):
+    def __init__(self, items, marked_with: str = "-"):
         """
 
         :param items: Array of items for generating the list.
         :type items: [str]
         :param marked_with: By default has the value of ``'-'``, can be ``'+'``, ``'*'``. If you want to generate
          an ordered list then set to ``'1'``.
         :type marked_with: str
         """
         super().__init__()
-        self.md_list = self._get_ordered_markdown_list(items) if marked_with == '1' else \
-            self._get_unordered_markdown_list(items, marked_with)
+        self.md_list = (
+            self._get_ordered_markdown_list(items)
+            if marked_with == "1"
+            else self._get_unordered_markdown_list(items, marked_with)
+        )
 
     def get_md(self) -> str:
         """Get the list in markdown format.
 
         :return:
         :rtype: str
         """
         return self.md_list
 
 
 class MDCheckbox(MDListHelper):
-    """This class allows to create checkbox MarkDown list.
-
-    """
+    """This class allows to create checkbox MarkDown list."""
 
-    def __init__(self, items: [str], checked: bool = False):
+    def __init__(self, items, checked: bool = False):
         """
 
         :param items: Array of items for generating the list.
         :type items: [str]
         :param checked: Set to ``True``, if you want that all items become checked. By default is set to ``False``.
         :type checked: bool
         """
         super().__init__()
-        self.checked = " " if not checked else 'x'
-        self.md_list = self._get_unordered_markdown_list(items, marker=f'- [{self.checked}]')
+        self.checked = " " if not checked else "x"
+        self.md_list = self._get_unordered_markdown_list(
+            items, marker=f"- [{self.checked}]"
+        )
 
     def get_md(self) -> str:
         return self.md_list
 
     def _add_new_item(self, item: str, marker: str):
-        item_with_hyphen = self._add_hyphen(item[2:], '- [x]') if self.__is_checked(item) \
+        item_with_hyphen = (
+            self._add_hyphen(item[2:], "- [x]")
+            if self.__is_checked(item)
             else self._add_hyphen(item, marker)
-        return self._n_spaces(4 * self.n_tabs) + item_with_hyphen + '\n'
+        )
+        return self._n_spaces(4 * self.n_tabs) + item_with_hyphen + "\n"
 
     @classmethod
     def __is_checked(cls, item: str) -> bool:
-        return item.startswith('x')
+        return item.startswith("x")
```

### Comparing `mdutils-1.5.1/mdutils/tools/Table.py` & `mdutils-1.6.0/mdutils/tools/Table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,93 @@
 # Python
 #
 # This module implements a text class that allows to modify and create text on Markdown files.
 #
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2020 Dídac Coll
-from typing import Optional, Union, Iterable
+from typing import Optional, Union, Iterable, List
 
 
 class Table:
-
     def __init__(self):
         self.rows = 0
         self.columns = 0
 
     @staticmethod
     def _align(columns: int, text_align: Optional[Union[str, Iterable]] = None) -> str:
-        """ This private method it's in charge of aligning text of a table.
+        """This private method it's in charge of aligning text of a table.
 
         - notes: more information about `text_align`
 
         :param columns: it is the number of columns.
         :param text_align: it is a string giving information about the alignment that is wanted.  text_align can take
                            the following parameters: ``'center'``, ``'right'`` and ``'left'``.
         :return: returns a string of type ``'| :---: | :---: | :---: |'``.
         :type columns: int
         :type text_align: str
         :rtype: str
 
         .. note:
         """
 
-        column_align_string = ''
-        ta2pat={ # text_align to pattern translator
-            'center': ' :---: |',
-            'left': ' :--- |',
-            'right': ' ---: |',
-            None: ' --- |'
+        column_align_string = ""
+        ta2pat = {  # text_align to pattern translator
+            "center": " :---: |",
+            "left": " :--- |",
+            "right": " ---: |",
+            None: " --- |",
         }
         if type(text_align) == str:
-            
-            text_align = [text_align.lower()]*columns
-            
+            text_align = [text_align.lower()] * columns
+
         elif text_align is None:
-            
-            text_align = [None]*columns
-            
+            text_align = [None] * columns
+
         else:
-            
-            text_align = list(text_align)[:columns] # make a local redimensionnable copy
-        
+            text_align = list(text_align)[
+                :columns
+            ]  # make a local redimensionnable copy
+
         if len(text_align) < columns:
-            
-            text_align += [None]*(columns-len(text_align))
-            
-        column_align_string = '|'
-        for i,ta in enumerate(text_align):
-            
-            if not ta is None:
-                
+            text_align += [None] * (columns - len(text_align))
+
+        column_align_string = "|"
+        for i, ta in enumerate(text_align):
+            if ta is not None:
                 ta = ta.lower()
-                
+
             if ta not in ta2pat:
-                
-                raise ValueError(f"text_align's expected value: 'right', 'center', 'left' or None , but in column {i+1} text_align = '{ta}'")
-            
+                raise ValueError(
+                    f"text_align's expected value: 'right', 'center', 'left' or None , but in column {i+1} text_align = '{ta}'"
+                )
+
             column_align_string += ta2pat[ta]
 
         return column_align_string
 
-    def create_table(self, columns: int, rows: int, text: [str], text_align: Optional[Union[str, list]] = None):
+    def create_table(
+        self,
+        columns: int,
+        rows: int,
+        text: List[str],
+        text_align: Optional[Union[str, list]] = None,
+    ):
         """This method takes a list of strings and creates a table.
 
             Using arguments ``columns`` and ``rows`` allows to create a table of *n* columns and *m* rows.
             The ``columns * rows`` operations has to correspond to the number of elements of ``text`` list argument.
 
         :param int columns: number of columns of the table.
         :param int rows: number of rows of the table.
         :param text: a list of strings.
         :type text: list of str
-        :param str_or_list text_align: text align argument. Values available are: ``'right'``, ``'center'``, ``'left'`` and ``None`` (default). If text_align is a list then individual alignment can be set for each column.
+        :param str_or_list text_align: text align argument.
+                                       Values available are: ``'right'``, ``'center'``, ``'left'`` and ``None`` (default).
+                                       If text_align is a list then individual alignment can be set for each column.
         :return: a markdown table.
         :rtype: str
 
 
         :Example:
         >>> from mdutils.tools.Table import Table
         >>> text_list = ['List of Items', 'Description', 'Result', 'Item 1', 'Description of item 1', '10', 'Item 2', 'Description of item 2', '0']
@@ -98,27 +102,27 @@
                "Item 1", "Description of Item 1", 10
                "Item 2", "Description of Item 2", 0
 
 
         """
         self.columns = columns
         self.rows = rows
-        table = '\n'
+        table = "\n"
         column_align_string = self._align(columns, text_align)
         index = 0
         if columns * rows == len(text):
             for row in range(rows + 1):
                 if row == 1:
                     table += column_align_string  # Row align, Example: '| :---: | :---: | ... | \n'
                 else:
-                    table += '|'
+                    table += "|"
                     for _ in range(columns):
-                        table += str(text[index]).replace("|", r"\|") + '|'
+                        table += str(text[index]).replace("|", r"\|") + "|"
                         index += 1
-                table += '\n'
+                table += "\n"
             return table
         else:
             raise ValueError("columns * rows is not equal to text length")
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `mdutils-1.5.1/mdutils/tools/TableOfContents.py` & `mdutils-1.6.0/mdutils/tools/TableOfContents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Python
 #
 # This module implements a text class that allows to modify and create text on Markdown files.
 #
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2020 Dídac Coll
+from typing import List
 import re
 
 
 class TableOfContents:
-    def _loop_through(self, elements, tab='', depth=1):
+    def _loop_through(self, elements, tab: str = "", depth: int = 1) -> str:
         """Method that go through a list of elements that contain strings and other list and return a string.
 
         The returned string is ready to be written in a markdown file in order to create a table of contents.
 
         :param elements: contain all the headers defined on the main class.
         :param tab: Inserts tabulations.
         :param depth: allows to include atx headers 1 through 6. Possible values: 1, 2, 3, 4, 5, or 6.
@@ -22,36 +23,51 @@
         :type depth: int
         :rtype: str
         """
         elements_to_string = ""
         for item in elements:
             if isinstance(item, list):
                 if item and depth > 1:
-                    elements_to_string += self._loop_through(item, tab=tab+'\t', depth=depth-1)
+                    elements_to_string += self._loop_through(
+                        item, tab=tab + "\t", depth=depth - 1
+                    )
             else:
-                elements_to_string += '\n' + tab + '* [' + item + '](#' \
-                                      + re.sub('[^a-z0-9_\-]', '', item.lower().replace(' ', '-')) + ')'
+                elements_to_string += (
+                    "\n"
+                    + tab
+                    + "* ["
+                    + item
+                    + "](#"
+                    + re.sub("[^a-z0-9_-]", "", item.lower().replace(" ", "-"))
+                    + ")"
+                )
 
         return elements_to_string
 
-    def create_table_of_contents(self, array_of_title_contents, depth=1):
+    def create_table_of_contents(
+        self, array_of_title_contents: List[str], depth: int = 1
+    ) -> str:
         """This method can create a table of contents using an array of the different titles. The depth can be changed.
         :param array_of_title_contents: a string list with the different headers.
         :type array_of_title_contents: list
         :param depth: allows to include atx headers 1 through 6. Possible values: 1, 2, 3, 4, 5, or 6.
         :type depth: int
         :return: return a string ready to be written to a Markdown file.
         :rtype: str
         """
-        if depth in range(1,7):
+        if depth in range(1, 7):
             table_of_contents = ""
-            table_of_contents += self._loop_through(array_of_title_contents, depth=depth)
-            table_of_contents += '\n'
+            table_of_contents += self._loop_through(
+                array_of_title_contents, depth=depth
+            )
+            table_of_contents += "\n"
             return table_of_contents
         else:
-            raise ValueError("depth's expected value: between 1 and 6, but depth = " + str(depth))
+            raise ValueError(
+                "depth's expected value: between 1 and 6, but depth = " + str(depth)
+            )
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `mdutils-1.5.1/mdutils/tools/TextUtils.py` & `mdutils-1.6.0/mdutils/tools/TextUtils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,103 +4,103 @@
 #
 # This file is part of mdutils. https://github.com/didix21/mdutils
 #
 # MIT License: (C) 2020 Dídac Coll
 
 
 class TextUtils:
-    """This class helps to create bold, italics and change color text.
-
-    """
+    """This class helps to create bold, italics and change color text."""
 
     @staticmethod
-    def bold(text):
+    def bold(text: str) -> str:
         """Bold text converter.
 
         :param text: a text string.
         :type text: str
         :return: a string like this example: ``'**text**'``
         :rtype: str"""
-        return '**' + text + '**'
+        return "**" + text + "**"
 
     @staticmethod
-    def italics(text):
+    def italics(text: str) -> str:
         """Italics text converter.
 
         :param text: a text string.
         :type text: str
         :return: a string like this example: ``'_text_'``
         :rtype: str"""
-        return '*' + text + '*'
+        return "*" + text + "*"
 
     @staticmethod
-    def inline_code(text):
+    def inline_code(text: str) -> str:
         """Inline code text converter.
 
         :param text: a text string.
         :type text: str
         :return: a string like this example: ``'``text``'``
         :rtype: str"""
-        return '``' + text + '``'
+        return "``" + text + "``"
 
     @staticmethod
-    def center_text(text):
+    def center_text(text: str) -> str:
         """Place a text string to center.
 
         :param text: a text string.
         :type text: str
         :return: a string like this exampple: ``'<center>text</center>'``
         """
-        return '<center>' + text + '</center>'
+        return "<center>" + text + "</center>"
 
     @staticmethod
-    def text_color(text, color="black"):
+    def text_color(text: str, color: str = "black") -> str:
         """Change text color.
 
         :param text: it is the text that will be changed its color.
         :param color: it is the text color: ``'orange'``, ``'blue'``, ``'red'``...
                       or a **RGB** color such as ``'#ffce00'``.
         :return: a string like this one: ``'<font color='color'>'text'</font>'``
         :type text: str
         :type color: str
         :rtype: str
         """
-        return '<font color="' + color + '">' + text + '</font>'
+        return '<font color="' + color + '">' + text + "</font>"
 
     @staticmethod
-    def text_external_link(text, link=''):
-        """ Using this method can be created an external link of a file or a web page.
+    def text_external_link(text: str, link: str = "") -> str:
+        """Using this method can be created an external link of a file or a web page.
 
         :param text: Text to be displayed.
         :type text: str
         :param link: External Link.
         :type link: str
         :return: return a string like this: ``'[Text to be shown](https://write.link.com)'``
         :rtype: str"""
 
-        return '[' + text + '](' + link + ')'
+        return "[" + text + "](" + link + ")"
 
     @staticmethod
-    def insert_code(code, language=''):
+    def insert_code(code: str, language: str = "") -> str:
         """This method allows to insert a peace of code.
 
         :param code: code string.
         :type code:str
         :param language: code language: python. c++, c#...
         :type language: str
         :return: markdown style.
         :rtype: str
         """
-        if language == '':
-            return '```\n' + code + '\n```'
+        if language == "":
+            return "```\n" + code + "\n```"
         else:
-            return '```' + language + '\n' + code + '\n```'
+            return "```" + language + "\n" + code + "\n```"
 
     @staticmethod
-    def text_format(text, bold_italics_code='', color='black', align=''):
+    def text_format(
+        text: str, bold_italics_code: str = "", color: str = "black", align: str = ""
+    ) -> str:
         """Text format helps to write multiple text format such as bold, italics and color.
 
         :param text: it is a string in which will be added the mew format
         :param bold_italics_code: using `'b'`: **bold**, `'i'`: _italics_ and `'c'`: `inline_code`.
         :param color: Can change text color. For example: 'red', 'green, 'orange'...
         :param align: Using this parameter you can align text.
         :return: return a string with the new text format.
@@ -114,39 +114,51 @@
 
         >>> from mdutils.tools.TextUtils import TextUtils
         >>> TextUtils.text_format(text='Some Text Here', bold_italics_code='bi', color='red', align='center')
         '***<center><font color="red">Some Text Here</font></center>***'
         """
         new_text_format = text
         if bold_italics_code:
-            if ('c' in bold_italics_code) or ('b' in bold_italics_code) or ('i' in bold_italics_code):
-                if 'c' in bold_italics_code:
+            if (
+                ("c" in bold_italics_code)
+                or ("b" in bold_italics_code)
+                or ("i" in bold_italics_code)
+            ):
+                if "c" in bold_italics_code:
                     new_text_format = TextUtils.inline_code(new_text_format)
             else:
-                raise ValueError("unexpected bold_italics_code value, options available: 'b', 'c' or 'i'.")
+                raise ValueError(
+                    "unexpected bold_italics_code value, options available: 'b', 'c' or 'i'."
+                )
 
-        if color != 'black':
+        if color != "black":
             new_text_format = TextUtils.text_color(new_text_format, color)
 
-        if align == 'center':
+        if align == "center":
             new_text_format = TextUtils.center_text(new_text_format)
 
         if bold_italics_code:
-            if ('c' in bold_italics_code) or ('b' in bold_italics_code) or ('i' in bold_italics_code):
-                if 'b' in bold_italics_code:
+            if (
+                ("c" in bold_italics_code)
+                or ("b" in bold_italics_code)
+                or ("i" in bold_italics_code)
+            ):
+                if "b" in bold_italics_code:
                     new_text_format = TextUtils.bold(new_text_format)
-                if 'i' in bold_italics_code:
+                if "i" in bold_italics_code:
                     new_text_format = TextUtils.italics(new_text_format)
             else:
-                raise ValueError("unexpected bold_italics_code value, options available: 'b', 'c' or 'i'.")
+                raise ValueError(
+                    "unexpected bold_italics_code value, options available: 'b', 'c' or 'i'."
+                )
 
         return new_text_format
 
     @staticmethod
-    def add_tooltip(link, tip):
+    def add_tooltip(link: str, tip: str) -> str:
         """
         :param link:
         :type link: str
         :param tip:
         :type tip: str
         return: ``link + "'" + format + "'"``
         """
```

### Comparing `mdutils-1.5.1/mdutils.egg-info/PKG-INFO` & `mdutils-1.6.0/mdutils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,106 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdutils
-Version: 1.5.1
+Version: 1.6.0
 Summary: Useful package for creating Markdown files while executing python code.
 Home-page: https://github.com/didix21/mdutils
 Author: Didac Coll
 Author-email: didaccoll_93@hotmail.com
 Maintainer: Didac Coll
 Maintainer-email: didaccoll_93@hotmail.com
 License: MIT
 Project-URL: Documentation, http://mdutils.readthedocs.io
 Project-URL: Say Thanks!, https://github.com/didix21/
 Project-URL: Source, https://github.com/didix21/mdutils
-Description: =======
-        mdutils
-        =======
-        |build-status| |documentation-status| |coverage-status|
-        
-        .. contents:: Table of Contents
-        
-        Overview
-        ========
-        This Python package contains a set of basic tools that can help to create a markdown file while running a Python code.
-        Thus, if you are executing a Python code and you save the result in a text file, Why not format it? So
-        using files such as Markdown can give a great look to those results. In this way, mdutils will make things easy for
-        creating Markdown files.
-        
-        - Project Homepage: https://github.com/didix21/mdutils
-        - Download Page: https://pypi.python.org/pypi/mdutils
-        - Documentation: http://mdutils.readthedocs.io/en/latest/
-        
-        MIT License, (C) 2018 Didac Coll <didaccoll_93@hotmail.com>
-        
-        Features
-        ========
-        There are some different features available on that version of mdutils:
-        
-        Writing and Reading Files
-        -------------------------
-        - Write and Read Markdown files.
-        - Append data to the end of a Markdown file.
-        - Use markers to place text.
-        
-        Markdown
-        --------
-        - Implemented method to give format to the text: bold, italics, change color...
-        - Align text.
-        - Add headers of levels 1 til 6 (atx style) or 1 and 2 (setext style).
-        - Create tables.
-        - Create a table of contents.
-        - Add Links.
-        - Add Lists.
-        - Add Markdown Images.
-        - Add Html Images.
-        
-        .. note::
-        
-            Some available features will depen on which CSS you are using. For example, GitHub do not allows to give color to text.
-        
-        
-        Installation
-        ============
-        Use pip to install mdutils:
-        
-        .. code:: bash
-        
-            $ pip install mdutils
-        
-        
-        
-        .. |build-status| image:: https://travis-ci.org/didix21/mdutils.svg?branch=master
-            :target: https://travis-ci.org/didix21/mdutils
-            :alt: Build Status
-        
-        .. |documentation-status| image:: https://readthedocs.org/projects/mdutils/badge/?version=latest
-            :target: http://mdutils.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. |coverage-status| image:: https://coveralls.io/repos/github/didix21/mdutils/badge.svg?branch=add-coveralls
-            :target: https://coveralls.io/github/didix21/mdutils?branch=add-coveralls
-            :alt: Coverage Status
-        
 Platform: Python 3.6
 Platform: Python 3.7
 Platform: Python 3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.txt
+
+=======
+mdutils
+=======
+|build-status| |documentation-status| |coverage-status|
+
+.. contents:: Table of Contents
+
+Overview
+========
+This Python package contains a set of basic tools that can help to create a markdown file while running a Python code.
+Thus, if you are executing a Python code and you save the result in a text file, Why not format it? So
+using files such as Markdown can give a great look to those results. In this way, mdutils will make things easy for
+creating Markdown files.
+
+- Project Homepage: https://github.com/didix21/mdutils
+- Download Page: https://pypi.python.org/pypi/mdutils
+- Documentation: http://mdutils.readthedocs.io/en/latest/
+
+MIT License, (C) 2018 Didac Coll <didaccoll_93@hotmail.com>
+
+Features
+========
+There are some different features available on that version of mdutils:
+
+Writing and Reading Files
+-------------------------
+- Write and Read Markdown files.
+- Append data to the end of a Markdown file.
+- Use markers to place text.
+
+Markdown
+--------
+- Implemented method to give format to the text: bold, italics, change color...
+- Align text.
+- Add headers of levels 1 til 6 (atx style) or 1 and 2 (setext style).
+- Create tables.
+- Create a table of contents.
+- Add Links.
+- Add Lists.
+- Add Markdown Images.
+- Add Html Images.
+
+.. note::
+
+    Some available features will depen on which CSS you are using. For example, GitHub do not allows to give color to text.
+
+
+Installation
+============
+
+Pip
+---
+Use pip to install mdutils:
+
+.. code:: bash
+
+    $ pip install mdutils
+
+Poetry
+------
+Use poetry to install mdutils:
+
+.. code:: bash
+
+    $ poetry add mdutils
+
+
+.. |build-status| image:: https://github.com/didix21/mdutils/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/didix21/mdutils
+    :alt: Build Status
+
+.. |documentation-status| image:: https://readthedocs.org/projects/mdutils/badge/?version=latest
+    :target: http://mdutils.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |coverage-status| image:: https://codecov.io/gh/didix21/mdutils/branch/master/graph/badge.svg?token=0DN72Z1B6V
+    :target: https://codecov.io/gh/didix21/mdutils
+    :alt: Coverage Status
```

### Comparing `mdutils-1.5.1/mdutils.egg-info/SOURCES.txt` & `mdutils-1.6.0/mdutils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ./doc/source/README.rst
 mdutils/__init__.py
 mdutils/mdutils.py
 mdutils.egg-info/PKG-INFO
 mdutils.egg-info/SOURCES.txt
@@ -17,8 +18,9 @@
 mdutils/tools/Html.py
 mdutils/tools/Image.py
 mdutils/tools/Link.py
 mdutils/tools/MDList.py
 mdutils/tools/Table.py
 mdutils/tools/TableOfContents.py
 mdutils/tools/TextUtils.py
-mdutils/tools/__init__.py
+mdutils/tools/__init__.py
+tests/test_mdutils.py
```

### Comparing `mdutils-1.5.1/setup.py` & `mdutils-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='mdutils',
-      version='1.5.1',
+      version='1.6.0',
       license='MIT',
       author='Didac Coll',
       author_email='didaccoll_93@hotmail.com',
       maintainer='Didac Coll',
       maintainer_email='didaccoll_93@hotmail.com',
       description='Useful package for creating Markdown files while executing python code.',
       long_description=open('./doc/source/README.rst').read(),
```


# Comparing `tmp/gqylpy_command-1.1.tar.gz` & `tmp/gqylpy_command-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_command-1.1.tar", last modified: Sun Oct 30 11:21:12 2022, max compression
+gzip compressed data, was "gqylpy_command-1.1.1.tar", last modified: Sat Apr 29 01:55:25 2023, max compression
```

## Comparing `gqylpy_command-1.1.tar` & `gqylpy_command-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:21:12.937067 gqylpy_command-1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11383 2022-10-30 11:21:02.000000 gqylpy_command-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-30 11:21:12.937067 gqylpy_command-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-10-30 11:21:02.000000 gqylpy_command-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:21:12.937067 gqylpy_command-1.1/gqylpy_command/
--rw-r--r--   0 runner    (1001) docker     (121)    10190 2022-10-30 11:21:02.000000 gqylpy_command-1.1/gqylpy_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9297 2022-10-30 11:21:02.000000 gqylpy_command-1.1/gqylpy_command/g command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:21:12.937067 gqylpy_command-1.1/gqylpy_command.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-30 11:21:12.000000 gqylpy_command-1.1/gqylpy_command.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-30 11:21:12.000000 gqylpy_command-1.1/gqylpy_command.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 11:21:12.000000 gqylpy_command-1.1/gqylpy_command.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-30 11:21:12.000000 gqylpy_command-1.1/gqylpy_command.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 11:21:12.937067 gqylpy_command-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-10-30 11:21:02.000000 gqylpy_command-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:55:25.141196 gqylpy_command-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-29 01:55:11.000000 gqylpy_command-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-29 01:55:25.137196 gqylpy_command-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 01:55:11.000000 gqylpy_command-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:55:25.137196 gqylpy_command-1.1.1/gqylpy_command/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-29 01:55:11.000000 gqylpy_command-1.1.1/gqylpy_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-29 01:55:11.000000 gqylpy_command-1.1.1/gqylpy_command/g command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:55:25.137196 gqylpy_command-1.1.1/gqylpy_command.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-29 01:55:25.000000 gqylpy_command-1.1.1/gqylpy_command.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 01:55:25.000000 gqylpy_command-1.1.1/gqylpy_command.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:55:25.000000 gqylpy_command-1.1.1/gqylpy_command.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 01:55:25.000000 gqylpy_command-1.1.1/gqylpy_command.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:55:25.141196 gqylpy_command-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-29 01:55:11.000000 gqylpy_command-1.1.1/setup.py
```

### Comparing `gqylpy_command-1.1/LICENSE` & `gqylpy_command-1.1.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022 GQYLPY <http://gqylpy.com>. All rights reserved.
+   Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_command-1.1/PKG-INFO` & `gqylpy_command-1.1.1/gqylpy_command.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: gqylpy_command
-Version: 1.1
+Name: gqylpy-command
+Version: 1.1.1
+Summary: 调用系统命令，基于内置库 subprocess。并提供了多种用于判断命令调用结果是否如期的方法。
 Home-page: http://gqylpy.com
 Author: 竹永康
-Author-email: gqylpy@outlook.com
+Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-command
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
@@ -15,31 +16,31 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-command.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-command/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_command)](https://pypi.org/project/gqylpy_command)
 [![License](https://img.shields.io/pypi/l/gqylpy_command)](https://github.com/gqylpy/gqylpy-command/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_command/month)](https://pepy.tech/project/gqylpy_command)
+[![Downloads](https://pepy.tech/badge/gqylpy_command)](https://pepy.tech/project/gqylpy_command)
 
 # gqylpy-command
 
-> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方法用于判断命令调用结果是否如期。
+> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方案用于判断命令调用结果是否如期。
 
 `pip3 install gqylpy_command`
 
 ```python
-from gqylpy_command import gcmd
+>>> from gqylpy_command import gcmd
 
-c = gcmd('hostname')
+>>> c = gcmd('hostname')
 
-status: bool = c.status
-output: str  = c.output
+>>> c.status_output
+(True, 'Alpha')
 ```
```

### Comparing `gqylpy_command-1.1/README.md` & `gqylpy_command-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-command.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-command/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_command)](https://pypi.org/project/gqylpy_command)
 [![License](https://img.shields.io/pypi/l/gqylpy_command)](https://github.com/gqylpy/gqylpy-command/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_command/month)](https://pepy.tech/project/gqylpy_command)
+[![Downloads](https://pepy.tech/badge/gqylpy_command)](https://pepy.tech/project/gqylpy_command)
 
 # gqylpy-command
 
-> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方法用于判断命令调用结果是否如期。
+> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方案用于判断命令调用结果是否如期。
 
 `pip3 install gqylpy_command`
 
 ```python
-from gqylpy_command import gcmd
+>>> from gqylpy_command import gcmd
 
-c = gcmd('hostname')
+>>> c = gcmd('hostname')
 
-status: bool = c.status
-output: str  = c.output
+>>> c.status_output
+(True, 'Alpha')
 ```
```

### Comparing `gqylpy_command-1.1/gqylpy_command.egg-info/PKG-INFO` & `gqylpy_command-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: gqylpy-command
-Version: 1.1
+Name: gqylpy_command
+Version: 1.1.1
+Summary: 调用系统命令，基于内置库 subprocess。并提供了多种用于判断命令调用结果是否如期的方法。
 Home-page: http://gqylpy.com
 Author: 竹永康
-Author-email: gqylpy@outlook.com
+Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-command
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
@@ -15,31 +16,31 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-command.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-command/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_command)](https://pypi.org/project/gqylpy_command)
 [![License](https://img.shields.io/pypi/l/gqylpy_command)](https://github.com/gqylpy/gqylpy-command/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_command/month)](https://pepy.tech/project/gqylpy_command)
+[![Downloads](https://pepy.tech/badge/gqylpy_command)](https://pepy.tech/project/gqylpy_command)
 
 # gqylpy-command
 
-> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方法用于判断命令调用结果是否如期。
+> 调用系统命令，它是对内置库 subprocess 的二次封装。在 `gcmd` 对象中，提供了多种方案用于判断命令调用结果是否如期。
 
 `pip3 install gqylpy_command`
 
 ```python
-from gqylpy_command import gcmd
+>>> from gqylpy_command import gcmd
 
-c = gcmd('hostname')
+>>> c = gcmd('hostname')
 
-status: bool = c.status
-output: str  = c.output
+>>> c.status_output
+(True, 'Alpha')
 ```
```

### Comparing `gqylpy_command-1.1/setup.py` & `gqylpy_command-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import setuptools
 import gqylpy_command as g
 
+with open(g.__file__, encoding='utf8') as f:
+    for line in f:
+        if line.startswith('@version: ', 4):
+            version = line.split()[-1]
+            break
+    author, email = f.readline().split(maxsplit=1)[-1].rstrip().split()
+    source = f.readline().split()[-1]
+
 setuptools.setup(
     name=g.__name__,
-    version='.'.join(str(n) for n in g.__version__),
-    author=g.__author__.split()[0],
-    author_email=g.__author__.split()[1][1:-1],
+    version=version,
+    author=author,
+    author_email=email,
     license='Apache 2.0',
     url='http://gqylpy.com',
-    project_urls={'Source': g.__source__},
+    project_urls={'Source': source},
+    description='调用系统命令，基于内置库 subprocess。并提供了多种用于判断命令调用结果'
+                '是否如期的方法。',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=[g.__name__],
-    python_requires='>=3.6',
+    python_requires='>=3.6, <4',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Topic :: Text Processing :: Indexing',
         'Topic :: Utilities',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


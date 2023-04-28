# Comparing `tmp/shellextools-0.14.tar.gz` & `tmp/shellextools-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellextools-0.14.tar", last modified: Fri Apr 28 23:03:09 2023, max compression
+gzip compressed data, was "shellextools-0.15.tar", last modified: Fri Apr 28 23:07:40 2023, max compression
```

## Comparing `shellextools-0.14.tar` & `shellextools-0.15.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.932038 shellextools-0.14/
--rw-rw-rw-   0        0        0     1148 2023-04-28 23:02:53.000000 shellextools-0.14/LICENSE.rst
--rw-rw-rw-   0        0        0      209 2023-04-28 23:02:51.000000 shellextools-0.14/MANIFEST.in
--rw-rw-rw-   0        0        0     3804 2023-04-28 23:03:09.932038 shellextools-0.14/PKG-INFO
--rw-rw-rw-   0        0        0     3154 2023-04-24 01:10:31.000000 shellextools-0.14/README.md
--rw-rw-rw-   0        0        0       85 2023-04-28 23:03:09.933036 shellextools-0.14/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-04-28 23:03:08.000000 shellextools-0.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.928049 shellextools-0.14/shellextools/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.14/shellextools/LICENSE
--rw-rw-rw-   0        0        0     3154 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/README.md
--rw-rw-rw-   0        0        0    51326 2023-04-28 23:02:03.000000 shellextools-0.14/shellextools/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/getmultifiles.py
--rw-rw-rw-   0        0        0     2555 2023-04-24 01:10:31.000000 shellextools-0.14/shellextools/loggax3.py
--rw-rw-rw-   0        0        0      248 2023-04-28 23:03:08.000000 shellextools-0.14/shellextools/requirements.txt
--rw-rw-rw-   0        0        0     9983 2023-04-28 23:03:08.000000 shellextools-0.14/shellextools/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-28 23:03:09.931041 shellextools-0.14/shellextools.egg-info/
--rw-rw-rw-   0        0        0     3804 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 23:03:09.000000 shellextools-0.14/shellextools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:07:40.584426 shellextools-0.15/
+-rw-rw-rw-   0        0        0     1148 2023-04-28 23:07:25.000000 shellextools-0.15/LICENSE.rst
+-rw-rw-rw-   0        0        0      209 2023-04-28 23:07:25.000000 shellextools-0.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     4196 2023-04-28 23:07:40.584426 shellextools-0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     3546 2023-04-28 23:04:00.000000 shellextools-0.15/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-28 23:07:40.585424 shellextools-0.15/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-04-28 23:07:39.000000 shellextools-0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:07:40.580437 shellextools-0.15/shellextools/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.15/shellextools/LICENSE
+-rw-rw-rw-   0        0        0     3546 2023-04-28 23:04:00.000000 shellextools-0.15/shellextools/README.md
+-rw-rw-rw-   0        0        0    51326 2023-04-28 23:02:03.000000 shellextools-0.15/shellextools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-24 01:10:31.000000 shellextools-0.15/shellextools/getmultifiles.py
+-rw-rw-rw-   0        0        0     2555 2023-04-24 01:10:31.000000 shellextools-0.15/shellextools/loggax3.py
+-rw-rw-rw-   0        0        0      248 2023-04-28 23:07:39.000000 shellextools-0.15/shellextools/requirements.txt
+-rw-rw-rw-   0        0        0     9983 2023-04-28 23:07:39.000000 shellextools-0.15/shellextools/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-28 23:07:40.583429 shellextools-0.15/shellextools.egg-info/
+-rw-rw-rw-   0        0        0     4196 2023-04-28 23:07:40.000000 shellextools-0.15/shellextools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-28 23:07:40.000000 shellextools-0.15/shellextools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:07:40.000000 shellextools-0.15/shellextools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-28 23:07:40.000000 shellextools-0.15/shellextools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 23:07:40.000000 shellextools-0.15/shellextools.egg-info/top_level.txt
```

### Comparing `shellextools-0.14/LICENSE.rst` & `shellextools-0.15/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/PKG-INFO` & `shellextools-0.15/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: shellextools
-Version: 0.14
-Summary: Adds Python functions/methods to the Windows context menu
-Home-page: https://github.com/hansalemaos/shellextools
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: Windows context menu,python,nutika
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here are 2 examples:
+### Here are some examples:
+
+
+
+https://github.com/hansalemaos/ripgrepgui
+
+[![](https://i.ytimg.com/vi/54XZXw1KOvQ/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLAsTyJc2bHqxjyDSqz29y_VQpVQ2A)](https://www.youtube.com/shorts/54XZXw1KOvQ)
 
 https://github.com/hansalemaos/rc_collage
 
 [![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
+[![](https://i.ytimg.com/vi/SPcOx8M4Wqo/oar2.jpg)](https://www.youtube.com/shorts/SPcOx8M4Wqo)
+
+https://github.com/githubrobbi/Ultra-Fast-File-Search
+
 
 ## Create a pyw file 
 
 ```python
 from PIL import Image
 from hackyargparser import add_sysargv
 from shellextools import (
```

### Comparing `shellextools-0.14/setup.py` & `shellextools-0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.14'''
+VERSION = '''0.15'''
 DESCRIPTION = '''Adds Python functions/methods to the Windows context menu'''
 
 # Setting up
 setup(
     name="shellextools",
     version=VERSION,
     license='MIT',
```

### Comparing `shellextools-0.14/shellextools/LICENSE` & `shellextools-0.15/shellextools/LICENSE`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/shellextools/__init__.py` & `shellextools-0.15/shellextools/__init__.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/shellextools/getmultifiles.py` & `shellextools-0.15/shellextools/getmultifiles.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/shellextools/loggax3.py` & `shellextools-0.15/shellextools/loggax3.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/shellextools/thirdparty.json` & `shellextools-0.15/shellextools/thirdparty.json`

 * *Files identical despite different names*

### Comparing `shellextools-0.14/shellextools.egg-info/PKG-INFO` & `shellextools-0.15/shellextools/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: shellextools
-Version: 0.14
-Summary: Adds Python functions/methods to the Windows context menu
-Home-page: https://github.com/hansalemaos/shellextools
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: Windows context menu,python,nutika
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here are 2 examples:
+### Here are some examples:
+
+
+
+https://github.com/hansalemaos/ripgrepgui
+
+[![](https://i.ytimg.com/vi/54XZXw1KOvQ/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLAsTyJc2bHqxjyDSqz29y_VQpVQ2A)](https://www.youtube.com/shorts/54XZXw1KOvQ)
 
 https://github.com/hansalemaos/rc_collage
 
 [![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
+[![](https://i.ytimg.com/vi/SPcOx8M4Wqo/oar2.jpg)](https://www.youtube.com/shorts/SPcOx8M4Wqo)
+
+https://github.com/githubrobbi/Ultra-Fast-File-Search
+
 
 ## Create a pyw file 
 
 ```python
 from PIL import Image
 from hackyargparser import add_sysargv
 from shellextools import (
```


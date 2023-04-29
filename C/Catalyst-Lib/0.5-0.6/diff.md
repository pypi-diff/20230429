# Comparing `tmp/Catalyst_Lib-0.5.tar.gz` & `tmp/Catalyst_Lib-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Catalyst_Lib-0.5.tar", last modified: Sat Apr 29 02:32:03 2023, max compression
+gzip compressed data, was "Catalyst_Lib-0.6.tar", last modified: Sat Apr 29 02:37:01 2023, max compression
```

## Comparing `Catalyst_Lib-0.5.tar` & `Catalyst_Lib-0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/
-drwxrwxrwx   0        0        0        0 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib/
--rw-rw-rw-   0        0        0     2559 2022-11-28 16:45:48.000000 Catalyst_Lib-0.5/Catalyst_Lib/UserProfile.py
--rw-rw-rw-   0        0        0     1025 2023-04-29 02:31:54.000000 Catalyst_Lib-0.5/Catalyst_Lib/__init__.py
--rw-rw-rw-   0        0        0     7664 2022-11-28 16:45:48.000000 Catalyst_Lib-0.5/Catalyst_Lib/colors.py
--rw-rw-rw-   0        0        0     1418 2022-11-15 19:04:12.000000 Catalyst_Lib-0.5/Catalyst_Lib/dictionaries.py
--rw-rw-rw-   0        0        0     1600 2022-11-28 16:45:48.000000 Catalyst_Lib-0.5/Catalyst_Lib/exporter.py
--rw-rw-rw-   0        0        0     5085 2022-11-16 14:01:48.000000 Catalyst_Lib-0.5/Catalyst_Lib/graphbuilder.py
--rw-rw-rw-   0        0        0    15802 2022-11-16 13:25:50.000000 Catalyst_Lib-0.5/Catalyst_Lib/htmlgen.py
--rw-rw-rw-   0        0        0     2119 2022-11-28 17:08:50.000000 Catalyst_Lib-0.5/Catalyst_Lib/lib.py
--rw-rw-rw-   0        0        0     4631 2022-12-05 17:55:22.000000 Catalyst_Lib-0.5/Catalyst_Lib/lists.py
--rw-rw-rw-   0        0        0     6155 2022-11-11 15:44:50.000000 Catalyst_Lib-0.5/Catalyst_Lib/multiLambda.py
--rw-rw-rw-   0        0        0     2034 2022-11-17 16:08:30.000000 Catalyst_Lib-0.5/Catalyst_Lib/progressBar.py
--rw-rw-rw-   0        0        0     3044 2022-11-11 15:44:50.000000 Catalyst_Lib-0.5/Catalyst_Lib/question.py
--rw-rw-rw-   0        0        0     8705 2022-11-11 15:44:50.000000 Catalyst_Lib-0.5/Catalyst_Lib/randomgen.py
--rw-rw-rw-   0        0        0     5740 2022-12-03 09:57:54.000000 Catalyst_Lib-0.5/Catalyst_Lib/table.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib.egg-info/
--rw-rw-rw-   0        0        0      899 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/Catalyst_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2023-04-26 04:40:00.000000 Catalyst_Lib-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      899 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-04-29 02:32:04.000000 Catalyst_Lib-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1722 2023-04-29 02:32:00.000000 Catalyst_Lib-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/
+drwxrwxrwx   0        0        0        0 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib/
+-rw-rw-rw-   0        0        0     2559 2022-11-28 16:45:48.000000 Catalyst_Lib-0.6/Catalyst_Lib/UserProfile.py
+-rw-rw-rw-   0        0        0      984 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/__init__.py
+-rw-rw-rw-   0        0        0     7664 2022-11-28 16:45:48.000000 Catalyst_Lib-0.6/Catalyst_Lib/colors.py
+-rw-rw-rw-   0        0        0     1418 2022-11-15 19:04:12.000000 Catalyst_Lib-0.6/Catalyst_Lib/dictionaries.py
+-rw-rw-rw-   0        0        0     1600 2022-11-28 16:45:48.000000 Catalyst_Lib-0.6/Catalyst_Lib/exporter.py
+-rw-rw-rw-   0        0        0     5085 2022-11-16 14:01:48.000000 Catalyst_Lib-0.6/Catalyst_Lib/graphbuilder.py
+-rw-rw-rw-   0        0        0    15802 2022-11-16 13:25:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/htmlgen.py
+-rw-rw-rw-   0        0        0     2119 2022-11-28 17:08:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/lib.py
+-rw-rw-rw-   0        0        0     4625 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/lists.py
+-rw-rw-rw-   0        0        0     6155 2022-11-11 15:44:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/multiLambda.py
+-rw-rw-rw-   0        0        0     2037 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/progressBar.py
+-rw-rw-rw-   0        0        0     3044 2022-11-11 15:44:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/question.py
+-rw-rw-rw-   0        0        0     8699 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/randomgen.py
+-rw-rw-rw-   0        0        0     5734 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/Catalyst_Lib/table.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/Catalyst_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-04-26 04:40:00.000000 Catalyst_Lib-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      899 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-04-29 02:37:02.000000 Catalyst_Lib-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1722 2023-04-29 02:36:50.000000 Catalyst_Lib-0.6/setup.py
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/UserProfile.py` & `Catalyst_Lib-0.6/Catalyst_Lib/UserProfile.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/__init__.py` & `Catalyst_Lib-0.6/Catalyst_Lib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 from . import colors, dictionaries, exporter, graphbuilder, htmlgen, lib, lists, multiLambda, progressBar, question, randomgen, table, UserProfile
 
 
 this = sys.modules[__name__]
 
 
 this.mode = "Production"
-this.__version__ = 0.5
+this.__version__ = 0.6
 
 
 def update_status():
     if this.mode == "Development":
         print("Catalyst Lib running in development mode")
         status = requests.get("https://pypi.python.org/pypi/Catalyst-Lib/json")
         if status.status_code == 200:
-            print(status.json().keys())
             if float(status.json()["info"]["version"]) > this.__version__:
                 print(f"Please update Catalyst Lib to the latest version ({status.json()['info']['version']})")
     if this.mode == "Production":
         pass
 
 
 def thankyou():
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/colors.py` & `Catalyst_Lib-0.6/Catalyst_Lib/colors.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/dictionaries.py` & `Catalyst_Lib-0.6/Catalyst_Lib/dictionaries.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/exporter.py` & `Catalyst_Lib-0.6/Catalyst_Lib/exporter.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/graphbuilder.py` & `Catalyst_Lib-0.6/Catalyst_Lib/graphbuilder.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/htmlgen.py` & `Catalyst_Lib-0.6/Catalyst_Lib/htmlgen.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/lib.py` & `Catalyst_Lib-0.6/Catalyst_Lib/lib.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/lists.py` & `Catalyst_Lib-0.6/Catalyst_Lib/lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from easylib import dictionaries
+from . import dictionaries
 
 
 def contains_duplicates(items: list):
     for x in items:
         if items.count(x) != 1:
             return True
     return False
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/multiLambda.py` & `Catalyst_Lib-0.6/Catalyst_Lib/multiLambda.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/progressBar.py` & `Catalyst_Lib-0.6/Catalyst_Lib/progressBar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import sys, time
+import sys
+import time
 from datetime import datetime
-from easylib.colors import color, colored
+
+from ..colors import color, colored
 
 
 def progressbar(it, colors: color = color(color=(0, 0, 0)), prefix: str = "", size: int = 60, out=sys.stdout):  # Python3.3+
     """
     It takes an iterable, and prints a progress bar to the console, with a percentage, and an estimate of how long it will
     take to complete
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/question.py` & `Catalyst_Lib-0.6/Catalyst_Lib/question.py`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/randomgen.py` & `Catalyst_Lib-0.6/Catalyst_Lib/randomgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable
 from random import choice
-from easylib.lib import split
+from ..lib import split
 
 class Generator:
 
     def __init__(self, length: int = 25, nums: list = None):
         """
         This function takes in two arguments, length and nums, and sets the length and nums attributes of the object to the
         values of the arguments
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib/table.py` & `Catalyst_Lib-0.6/Catalyst_Lib/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 "─│┌┐└┘├┤┬┼┴═║╒╓╔╕╖╗╘╙╚╛╜╝╞╟╠╡╢╣╤╥╦╧╨╩╪╫╬"
-from easylib.lists import contains_duplicates
+from ..lists import contains_duplicates
 
 """
 print("┌────────────────────────────────────┐")
 print("│                                    │")
 print("└────────────────────────────────────┘")
 print("")
 print("╔════════════════════════════════════╗")
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib.egg-info/PKG-INFO` & `Catalyst_Lib-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Catalyst-Lib
-Version: 0.5
+Name: Catalyst_Lib
+Version: 0.6
 Summary: The all in one python library you need
 Home-page: https://github.com/Catalyst-Studio/Lib_Files
 Download-URL: https://github.com/Catalyst-Studio/Lib_Files/
 Author: Catalyst Studios
 Author-email: help@catalyst-studios.cc
 License: Apache License 2.0
 Keywords: library,easy,allinone
```

### Comparing `Catalyst_Lib-0.5/Catalyst_Lib.egg-info/SOURCES.txt` & `Catalyst_Lib-0.6/Catalyst_Lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/LICENSE.txt` & `Catalyst_Lib-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Catalyst_Lib-0.5/PKG-INFO` & `Catalyst_Lib-0.6/Catalyst_Lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Catalyst_Lib
-Version: 0.5
+Name: Catalyst-Lib
+Version: 0.6
 Summary: The all in one python library you need
 Home-page: https://github.com/Catalyst-Studio/Lib_Files
 Download-URL: https://github.com/Catalyst-Studio/Lib_Files/
 Author: Catalyst Studios
 Author-email: help@catalyst-studios.cc
 License: Apache License 2.0
 Keywords: library,easy,allinone
```

### Comparing `Catalyst_Lib-0.5/setup.py` & `Catalyst_Lib-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Catalyst_Lib',  # How you named your package folder (MyLib)
     packages=['Catalyst_Lib'],  # Chose the same as "name"
-    version='0.5',  # Start with a small number and increase it with every change you make
+    version='0.6',  # Start with a small number and increase it with every change you make
     license='Apache License 2.0',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='The all in one python library you need',  # Give a short description about your library
     author='Catalyst Studios',  # Type in your name
     author_email='help@catalyst-studios.cc',  # Type in your E-Mail
     url='https://github.com/Catalyst-Studio/Lib_Files',  # Provide either the link to your github or to your website
     download_url='https://github.com/Catalyst-Studio/Lib_Files/',  # I explain this later on
     keywords=["library", "easy", "allinone"],  # Keywords that define your package best
```


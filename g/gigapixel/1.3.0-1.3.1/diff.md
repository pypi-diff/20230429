# Comparing `tmp/gigapixel-1.3.0.tar.gz` & `tmp/gigapixel-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigapixel-1.3.0.tar", last modified: Sun Apr  9 11:47:45 2023, max compression
+gzip compressed data, was "gigapixel-1.3.1.tar", last modified: Sat Apr 29 09:16:55 2023, max compression
```

## Comparing `gigapixel-1.3.0.tar` & `gigapixel-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 11:47:35.000000 gigapixel-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-09 11:47:45.346704 gigapixel-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-09 11:47:35.000000 gigapixel-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/gigapixel/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/gigapixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-09 11:47:35.000000 gigapixel-1.3.0/gigapixel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:47:45.346704 gigapixel-1.3.0/gigapixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:47:45.000000 gigapixel-1.3.0/gigapixel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-09 11:47:35.000000 gigapixel-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 11:47:45.346704 gigapixel-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-09 11:47:35.000000 gigapixel-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 09:16:42.000000 gigapixel-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 09:16:55.413786 gigapixel-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-29 09:16:42.000000 gigapixel-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/gigapixel/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/gigapixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/gigapixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 09:16:42.000000 gigapixel-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 09:16:55.417786 gigapixel-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-29 09:16:42.000000 gigapixel-1.3.1/setup.py
```

### Comparing `gigapixel-1.3.0/LICENSE` & `gigapixel-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigapixel-1.3.0/PKG-INFO` & `gigapixel-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6** of **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.3.0 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.3.1 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -16,18 +16,18 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6** of **newer** required ## Installation Install the current version with
-[PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
-``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+**v6.3.3** or **newer** required ## Installation Install the current version
+with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
+U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
+method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
 image.jpg') output_path = app.process(image, scale=Scale.X2,
```

### Comparing `gigapixel-1.3.0/README.md` & `gigapixel-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6** of **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
```

#### html2text {}

```diff
@@ -2,18 +2,18 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6** of **newer** required ## Installation Install the current version with
-[PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
-``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+**v6.3.3** or **newer** required ## Installation Install the current version
+with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
+U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
+method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
 image.jpg') output_path = app.process(image, scale=Scale.X2,
```

### Comparing `gigapixel-1.3.0/gigapixel/gigapixel.py` & `gigapixel-1.3.1/gigapixel/gigapixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     X6 = "6x"
 
 
 class Mode(Enum):
     STANDARD = "Standard"
     Lines = "Lines"
     ART_AND_CG = "Art & CG"
-    LOW_RESOLUTION = "Low Resolution"
+    HIGH_QUALITY = "HQ"
+    LOW_RESOLUTION = "Low Res"
     VERY_COMPRESSED = "Very Compressed"
 
 
 class OutputFormat(Enum):
     PRESERVE_SOURCE_FORMAT = "Preserve Source Format"
     JPG = "JPG"
     JPEG = "JPEG"
```

### Comparing `gigapixel-1.3.0/gigapixel/logging.py` & `gigapixel-1.3.1/gigapixel/logging.py`

 * *Files identical despite different names*

### Comparing `gigapixel-1.3.0/gigapixel.egg-info/PKG-INFO` & `gigapixel-1.3.1/gigapixel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6** of **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.3.0 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.3.1 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -16,18 +16,18 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6** of **newer** required ## Installation Install the current version with
-[PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -U gigapixel
-``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()` method to
-enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
+**v6.3.3** or **newer** required ## Installation Install the current version
+with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
+U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
+method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
 image.jpg') output_path = app.process(image, scale=Scale.X2,
```

### Comparing `gigapixel-1.3.0/setup.py` & `gigapixel-1.3.1/setup.py`

 * *Files identical despite different names*


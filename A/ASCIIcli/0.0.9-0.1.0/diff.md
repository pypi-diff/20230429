# Comparing `tmp/ASCIIcli-0.0.9.tar.gz` & `tmp/ASCIIcli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.9.tar", last modified: Fri Apr 28 09:26:49 2023, max compression
+gzip compressed data, was "ASCIIcli-0.1.0.tar", last modified: Sat Apr 29 12:22:00 2023, max compression
```

## Comparing `ASCIIcli-0.0.9.tar` & `ASCIIcli-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.914813 ASCIIcli-0.0.9/ASCIIcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/ASCIIcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 12:22:00.000000 ASCIIcli-0.1.0/ASCIIcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/src/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:22:00.384285 ASCIIcli-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-29 12:21:49.000000 ASCIIcli-0.1.0/tests/tests.py
```

### Comparing `ASCIIcli-0.0.9/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-Metadata-Version: 2.1
-Name: ASCIIcli
-Version: 0.0.9
-Summary: A command-line tool that converts images to ASCII art.
-Home-page: https://github.com/mrq-andras/asciicli
-Author: mrq-andras
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+---
+  
+"   35005550    22           666     666             165         "  
+"  002          77    003    555     555             350         "  
+" 056                155677  555     555             3554 337    "  
+" 053   89889   00   4559    55555555555  006   400  3557   008  "  
+" 059     300   00    051    555     555  059   700  350    850  "  
+" 3007    700   00    053    555     555  059   400  350    950  "  
+"   900988500   00    90034  000     000  800371650  205847805   "  
+  
+---
 
 # Command Line ASCII Art Generator
 
 ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
 
----
-
 ## Installation & Building
 
 ### PIP
 
 The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
 You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
 
@@ -30,29 +25,29 @@
 
 If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
 
 ---
 
 ## Usage
 
-`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
+`asciicli [-h] [--percent] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
-Set 1: A -> Z  
-Set 2: 0 -> 9  
+Set 1: A --> Z  
+Set 2: 0 --> 9  
 Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
 Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
 Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
 
-**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
+**_NOTE: SET 5 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
-If you have downloaded the application through pip input the following command in the terminal:
-`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+If you have downloaded the application through pip input the following command in the terminal:  
+`asciicli --percent 20 --set 1 --random True C:/full/path/to/your/image`
 
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
-`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli  
+`.\path\to\asciicli.exe --percent 20 --set 1 --random True C:/full/path/to/your/image`
 
-This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
+Assuming the file is 1024x219, this command will generate a .txt file that is 21 lines long with each line taking up 201 characters using the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
 
 Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
 
 ---
 [`LICENSE`](./LICENSE)
```

### Comparing `ASCIIcli-0.0.9/LICENSE` & `ASCIIcli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.9/setup.py` & `ASCIIcli-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """
 This file is the setup script for the ASCIIcli module.
 This module provides a command line tool for converting images to ASCII art.
 
-To build:
+For manual uploading:
 `py -m build`
-
-To build EXE:
-`pyinstaller --onefile path/to/__main__.py`
-
-To distribute:
 `twine upload dist/*`
+`pyinstaller --onefile path/to/__main__.py`
 """
 
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ASCIIcli",
     author="mrq-andras",
-    version="0.0.9",
+    version="0.1.0",
     # needs to be wherever __init__.py is
     packages=['src'],
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -38,9 +34,9 @@
             "asciicli=src.__main__:main"
         ]
     },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/asciicli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
-    readme = "README.md"
+    readme="README.md"
 )
```

### Comparing `ASCIIcli-0.0.9/src/__main__.py` & `ASCIIcli-0.1.0/src/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,15 @@
                         help="Character set to use for the ASCII art (1 -> 5)",)
     parser.add_argument("--random", type=bool, default=False,
                         help="Character set is scrambled")
     parser.add_argument("--invert", type=bool, default=False,
                         help="Output is inverted")
     parser.add_argument("--darkness", type=int, default=100,
                         help="Darkness of line-art")
-    parser.add_argument("--width", type=int, default=62,
-                        help="The width of the output")
-    parser.add_argument("--height", type=int, default=26,
+    parser.add_argument("--percent", type=int,
                         help="The height of the output")
     args = parser.parse_args()
 
     # print out the chosen options
     print_cmd(args)
     # call the conversion function from ascii.py
     convert_to_ascii(args)
```

### Comparing `ASCIIcli-0.0.9/tests/tests.py` & `ASCIIcli-0.1.0/tests/tests.py`

 * *Files identical despite different names*


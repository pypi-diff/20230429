# Comparing `tmp/UzbekLemmatizer-1.0.1.tar.gz` & `tmp/UzbekLemmatizer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekLemmatizer-1.0.1.tar", last modified: Sat Mar 26 12:19:16 2022, max compression
+gzip compressed data, was "UzbekLemmatizer-1.0.2.tar", last modified: Sat Apr 29 05:55:59 2023, max compression
```

## Comparing `UzbekLemmatizer-1.0.1.tar` & `UzbekLemmatizer-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/
--rw-rw-r--   0 maksud    (1000) maksud    (1000)     1073 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.1/LICENSE
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/PKG-INFO
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      520 2022-03-05 06:43:33.000000 UzbekLemmatizer-1.0.1/README.md
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      103 2022-03-05 06:39:40.000000 UzbekLemmatizer-1.0.1/pyproject.toml
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      648 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/setup.cfg
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      871 2022-03-26 12:12:06.000000 UzbekLemmatizer-1.0.1/setup.py
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.508422 UzbekLemmatizer-1.0.1/src/
-drwxrwxr-x   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:19:16.512422 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      623 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/PKG-INFO
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      335 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/SOURCES.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      175 2022-03-26 10:57:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/UzbekLemmatizer.py
--rw-rw-r--   0 maksud    (1000) maksud    (1000)        0 2022-03-26 12:15:38.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/__init__.py
--rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/dependency_links.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)        1 2022-03-26 12:19:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.egg-info/top_level.txt
--rw-rw-r--   0 maksud    (1000) maksud    (1000)      175 2022-03-26 10:57:16.000000 UzbekLemmatizer-1.0.1/src/UzbekLemmatizer.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/
+-rw-rw-rw-   0        0        0     1109 2023-04-29 04:36:11.000000 UzbekLemmatizer-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-04-29 04:49:41.000000 UzbekLemmatizer-1.0.2/README.md
+-rw-rw-rw-   0        0        0      528 2023-04-29 05:55:24.000000 UzbekLemmatizer-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-04-29 05:54:18.000000 UzbekLemmatizer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/
+-rw-rw-rw-   0        0        0     4898 2023-04-29 04:10:27.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/UzbekLemmatizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 04:40:30.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/__init__.py
+-rw-rw-rw-   0        0        0     4035 2023-04-29 04:06:11.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/fsms.xml
+-rw-rw-rw-   0        0        0    53767 2023-04-08 11:23:16.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer/suffixes.xml
+drwxrwxrwx   0        0        0        0 2023-04-29 05:55:59.902086 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 05:55:59.000000 UzbekLemmatizer-1.0.2/src/UzbekLemmatizer.egg-info/top_level.txt
```

### Comparing `UzbekLemmatizer-1.0.1/LICENSE` & `UzbekLemmatizer-1.0.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+@@ -0,0 +1,21 @@
+MIT License
+
+Copyright (c) 2023 Maksud Sharipov
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `UzbekLemmatizer-1.0.1/setup.py` & `UzbekLemmatizer-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="UzbekLemmatizer",
-    version="1.0.1",
-    author="Maksud Sharipov",
-    author_email="maqsbek72@gmail.com",
-    description="Uzbek Lemmatizer for Python",
-    long_description="The Uzbek Lemmation algorithm was created by [Maksud Sharipov].",
-    long_description_content_type="text/markdown",
-    url="https://github.com/MaksudSharipov/UzbekLemmatizer",
-    project_urls={
-        "Bug Tracker": "https://github.com/MaksudSharipov/UzbekLemmatizer",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
+import setuptools
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="UzbekLemmatizer",
+    version="1.0.2",
+    author="Maksud Sharipov, Ollabergan Yuldashov",
+    author_email="maqsbek72@gmail.com, ollaberganyuldashov@gmail.com",
+    description="Uzbek Lemmatizer for Python. A Python package to lemmatize Uzbek words.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/MaksudSharipov/UzbekLemmatizer",
+    project_urls={
+        "Bug Tracker": "https://github.com/MaksudSharipov/UzbekLemmatizer/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    keywords=['python', 'UzbekLemmatizer', 'uzbek words', 'Lemmatizer'],
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    install_requires=[],
+    python_requires=">=3.6",
+    include_package_data=True,
+    package_data={"": ["*.xml"]},
+    #package_data={"": ["cyr_exwords.csv", "lat_exwords.csv"],},
 )
```


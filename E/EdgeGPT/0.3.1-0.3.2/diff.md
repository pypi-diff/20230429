# Comparing `tmp/EdgeGPT-0.3.1.tar.gz` & `tmp/EdgeGPT-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.1.tar", last modified: Fri Apr 28 13:59:43 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.2.tar", last modified: Sat Apr 29 13:41:32 2023, max compression
```

## Comparing `EdgeGPT-0.3.1.tar` & `EdgeGPT-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-28 13:59:42.000000 EdgeGPT-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.081182 EdgeGPT-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:43.085182 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 13:59:43.000000 EdgeGPT-0.3.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 13:59:13.000000 EdgeGPT-0.3.1/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:41:32.422943 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 13:41:32.000000 EdgeGPT-0.3.2/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 13:40:56.000000 EdgeGPT-0.3.2/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.1/LICENSE` & `EdgeGPT-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.1/PKG-INFO` & `EdgeGPT-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.1
+Version: 0.3.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.1/README.md` & `EdgeGPT-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.1/setup.py` & `EdgeGPT-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.1",
+    version="0.3.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.2/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.1
+Version: 0.3.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.1/src/EdgeGPT.py` & `EdgeGPT-0.3.2/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,19 +207,15 @@
         self.struct = {
             "arguments": [
                 {
                     "source": "cib",
                     "optionsSets": options,
                     "allowedMessageTypes": [
                         "Chat",
-                        "InternalSearchQuery",
-                        "InternalSearchResult",
                         "Disengaged",
-                        "InternalLoaderMessage",
-                        "RenderCardRequest",
                         "AdsQuery",
                         "SemanticSerp",
                         "GenerateContentQuery",
                         "SearchQuery",
                     ],
                     "sliceIds": [
                         "chk1cf",
@@ -382,15 +378,15 @@
                     "messages",
                 ):
                     try:
                         if not draw:
                             resp_txt = response["arguments"][0]["messages"][0][
                                 "adaptiveCards"
                             ][0]["body"][0].get("text")
-                            if(resp_txt == None):
+                            if resp_txt is None:
                                 resp_txt = ""
                         yield False, resp_txt
                     except Exception as exc:
                         print(exc)
                         if not draw:
                             continue
                         for item in cookies:
```


# Comparing `tmp/sweetbean-0.0.8.tar.gz` & `tmp/sweetbean-0.0.9.tar.gz`

## Comparing `sweetbean-0.0.8.tar` & `sweetbean-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 sweetbean-0.0.8/.gitattributes
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 sweetbean-0.0.8/example.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sweetbean-0.0.8/example_2.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 sweetbean-0.0.8/index.html
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sweetbean-0.0.8/main.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 sweetbean-0.0.8/test.js
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 sweetbean-0.0.8/sweetbean/__init__.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 sweetbean-0.0.8/sweetbean/primitives.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sweetbean-0.0.8/sweetbean/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sweetbean-0.0.8/sweetbean/examples/cepeda_et_all_1999/code.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 sweetbean-0.0.8/sweetbean/examples/cepeda_et_all_1999/text
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 sweetbean-0.0.8/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sweetbean-0.0.8/LICENCE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 sweetbean-0.0.8/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sweetbean-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 sweetbean-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 sweetbean-0.0.9/.gitattributes
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 sweetbean-0.0.9/example.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 sweetbean-0.0.9/example_2.py
+-rw-r--r--   0        0        0    45301 2020-02-02 00:00:00.000000 sweetbean-0.0.9/geckodriver.log
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 sweetbean-0.0.9/index.html
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sweetbean-0.0.9/main.py
+-rw-r--r--   0        0        0    19847 2020-02-02 00:00:00.000000 sweetbean-0.0.9/screenshot.png
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 sweetbean-0.0.9/test.html
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 sweetbean-0.0.9/test.js
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sweetbean-0.0.9/test.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/__init__.py
+-rw-r--r--   0        0        0    18702 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/fixation_screenshot.png
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/geckodriver.log
+-rw-r--r--   0        0        0    24007 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/primitives.py
+-rw-r--r--   0        0        0   110559 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/stimulus_timeline.png
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/examples/cepeda_et_all_1999/code.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 sweetbean-0.0.9/sweetbean/examples/cepeda_et_all_1999/text
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 sweetbean-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sweetbean-0.0.9/LICENCE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 sweetbean-0.0.9/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sweetbean-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 sweetbean-0.0.9/PKG-INFO
```

### Comparing `sweetbean-0.0.8/sweetbean/util.py` & `sweetbean-0.0.9/sweetbean/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
            '<head>\n' \
            '<title>My awesome expmeriment</title>' \
            '<script src="https://unpkg.com/jspsych@7.3.1"></script>\n' \
            '<script src="https://unpkg.com/@jspsych/plugin-html-keyboard-response@1.1.2"></script>\n' \
            '<link href="https://unpkg.com/jspsych@7.3.1/css/jspsych.css" rel="stylesheet" type="text/css"/>\n' \
            '<style>\n' \
            'body {background: #000; color: #fff;}\n' \
-           'div {font-size:24pt}' \
+           'div {font-size:72pt}' \
            '.sweetbean-square {width:10vw; height:10vw}' \
            '.sweetbean-circle {width:10vw; height:10vw; border-radius:50%}' \
            '.sweetbean-triangle {width:0; height: 0; border-left: 5vw solid transparent; border-right: 5vw solid transparent}' \
            '.feedback-screen-red {position:absolute; left:0; top:0; width:100vw; height: 100vh; background: red}' \
            '.feedback-screen-green {position:absolute; left:0; top: 0; width:100vw; height: 100vh; background: green}' \
            '</style>\n' \
            '</head>\n' \
```

### Comparing `sweetbean-0.0.8/sweetbean/examples/cepeda_et_all_1999/text` & `sweetbean-0.0.9/sweetbean/examples/cepeda_et_all_1999/text`

 * *Files identical despite different names*

### Comparing `sweetbean-0.0.8/LICENCE` & `sweetbean-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `sweetbean-0.0.8/README.md` & `sweetbean-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sweetbean-0.0.8/pyproject.toml` & `sweetbean-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 
 [project]
 name="sweetbean"
-version="0.0.8"
+version="0.0.9"
 authors=[{name="Younes Strittmatter", email="younes_strittmatter@brown.edu"},]
 description="declarative language in python for creating jsPsych experiments."
 requires-python= ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `sweetbean-0.0.8/PKG-INFO` & `sweetbean-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetbean
-Version: 0.0.8
+Version: 0.0.9
 Summary: declarative language in python for creating jsPsych experiments.
 Project-URL: Homepage, https://github.com/AutoResearch/sweetbean
 Project-URL: Bug Tracker, https://github.com/AutoResearch/sweetbean/issues
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweetbean Version: 0.0.8 Summary: declarative
+Metadata-Version: 2.1 Name: sweetbean Version: 0.0.9 Summary: declarative
 language in python for creating jsPsych experiments. Project-URL: Homepage,
 https://github.com/AutoResearch/sweetbean Project-URL: Bug Tracker, https://
 github.com/AutoResearch/sweetbean/issues Author-email: Younes Strittmatter
 brown.edu> License-File: LICENCE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown # sweetBean A declarative language in python for creating jsPsych
```


# Comparing `tmp/datamachine-0.0.7.tar.gz` & `tmp/datamachine-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.7.tar", last modified: Sat Apr 29 00:18:44 2023, max compression
+gzip compressed data, was "datamachine-0.0.8.tar", last modified: Sat Apr 29 02:42:23 2023, max compression
```

## Comparing `datamachine-0.0.7.tar` & `datamachine-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.460610 datamachine-0.0.7/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3657 2023-04-29 00:18:44.461425 datamachine-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3041 2023-04-28 23:48:04.000000 datamachine-0.0.7/README.md
--rw-rw-rw-   0        0        0      652 2023-04-29 00:17:55.000000 datamachine-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      599 2023-04-29 00:18:44.462449 datamachine-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.443231 datamachine-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.449320 datamachine-0.0.7/src/datamachine/
--rw-rw-rw-   0        0        0      270 2023-04-28 14:00:39.000000 datamachine-0.0.7/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0    10918 2023-04-29 00:15:15.000000 datamachine-0.0.7/src/datamachine/_modular.py
--rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.7/src/datamachine/xxx.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.460610 datamachine-0.0.7/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.856263 datamachine-0.0.8/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3515 2023-04-29 02:42:23.856263 datamachine-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3033 2023-04-29 02:40:44.000000 datamachine-0.0.8/README.md
+-rw-rw-rw-   0        0        0      520 2023-04-29 02:41:53.000000 datamachine-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      599 2023-04-29 02:42:23.857470 datamachine-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.834691 datamachine-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.840592 datamachine-0.0.8/src/datamachine/
+-rw-rw-rw-   0        0        0      271 2023-04-29 02:02:57.000000 datamachine-0.0.8/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0    11385 2023-04-29 02:39:59.000000 datamachine-0.0.8/src/datamachine/_modular.py
+-rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.8/src/datamachine/xxx.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.855342 datamachine-0.0.8/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0     3515 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.7/LICENSE` & `datamachine-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.7/PKG-INFO` & `datamachine-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.7
+Version: 0.0.8
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="left">
+<p align="left" style="width: 20%; max-width: 240px; min-width: 80px;" >
   <img src="https://storage.googleapis.com/benevolent-machines/bm.svg" 
-       style="width: 20%; max-width: 240px; min-width: 80px;" 
        title="BenevolentMachines.Org">
 </p>
 
 # datamachine 
 
 ## Welcome to the Machine!
```

### Comparing `datamachine-0.0.7/README.md` & `datamachine-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-<p align="left">
+<p align="left" style="width: 20%; max-width: 240px; min-width: 80px;" >
   <img src="https://storage.googleapis.com/benevolent-machines/bm.svg" 
-       style="width: 20%; max-width: 240px; min-width: 80px;" 
        title="BenevolentMachines.Org">
 </p>
 
 # datamachine 
 
 ## Welcome to the Machine!
```

### Comparing `datamachine-0.0.7/pyproject.toml` & `datamachine-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `datamachine-0.0.7/setup.cfg` & `datamachine-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 370d  version = 0.0.7.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
```

### Comparing `datamachine-0.0.7/src/datamachine/_modular.py` & `datamachine-0.0.8/src/datamachine/_modular.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "folder": DEFAULT["folder"],
     "library": DEFAULT["library"],
     "index": DEFAULT["index"],
     "process": str(os.getpid()),
     "invoker": None,
     "params": None,
     "notebooks": [],
+    "trace": True,
 }
 
 
 def _cache_notebook(notebook):
 
     if not os.path.exists(CURRENT["folder"]):
         os.makedirs(CURRENT["folder"])
@@ -118,19 +119,21 @@
                 processes.append(str(process.pid))
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
     return processes
 
 
 def _execute_enter(invoker):
+    _trace("_execute_enter(" + str(invoker) + ")")
     CURRENT["invoker"] = invoker
     path = CURRENT["folder"] + os.path.sep + "d_" + str(invoker) + "_execute.json"
     with open(path, encoding="utf-8") as file_in:
         req = json.loads(file_in.read())
         CURRENT["params"] = req["params"]
+    _trace(str(CURRENT["params"]))
 
 
 def _execute_stylings(html_data):
     html_data = html_data.replace(
         "</head>",
         """
         <style>
@@ -186,23 +189,39 @@
         idx = import_notebook(index)
         library_path = idx.LIBRARIES[library]["path"]
     lib = import_notebook(library_path)
     return _cache_notebook(lib.NOTEBOOKS[path]["path"])
 
 
 def _trace(line):
-    time_stamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S  ")
-    with open("request.txt", "a", encoding="utf-8") as file_out:
-        file_out.write(time_stamp + line + "\n")
+    if CURRENT["trace"] is True:
+        path = f"{CURRENT['folder']}{os.path.sep}d_{CURRENT['process']}_trace.txt"
+        print(path)
+        time_stamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S  ")
+        with open(path, "a+", encoding="utf-8") as file_out:
+            file_out.write(time_stamp + line + "\n")
+
+
+def _trace_off():
+    CURRENT["trace"] = False
+
+
+def _trace_on():
+    CURRENT["trace"] = True
 
 
 def execute_notebook(
     notebook=None, library=None, index=None, html=None, params=None, force_reload=False,
 ):
     """Execute a notebook"""
+
+    if not os.path.exists(CURRENT["folder"]):
+        os.makedirs(CURRENT["folder"])
+
+    _trace("execute_notebook('" + str(notebook) + "')")
     nbo = _get_notebook(notebook, library, index, force_reload=force_reload)
 
     request = {  # pass to the executed notebook
         "notebook": notebook,
         "library": library,
         "index": index,
         "html": html,
@@ -221,14 +240,15 @@
         code = os.linesep.join(
             [
                 "import datamachine as dm",
                 "#import src.datamachine as dm",
                 "dm._execute_enter('" + CURRENT["process"] + "')",
             ]
         )
+
         first_cell = nbformat.v4.new_code_cell(code)
         notebook_object.cells.insert(0, first_cell)
         execute_preprocessor = ExecutePreprocessor(timeout=600, kernel_name="python3")
         execute_preprocessor.preprocess(notebook_object)
 
         if html is not None:
             html_exporter = HTMLExporter()
@@ -238,28 +258,27 @@
             with open(html, "w", encoding="utf-8") as file_out:
                 file_out.write(html_data)
 
 
 def execute_params(params):
     """Set parameters"""
 
-    if CURRENT["invoker"] is None: # inside execute
+    if CURRENT["invoker"] is None:  # inside execute
         return params
 
     path = f"{CURRENT['folder']}{os.path.sep}d_{CURRENT['invoker']}_execute.json"
     if not os.path.exists(path):
         return params
 
     with open(path, encoding="utf-8") as file_in:
         request = file_in.read()
         req = json.loads(request)
         return req["params"]
 
 
-
 def import_notebook(
     notebook=None, library=None, index=None, force_reload=False,
 ):
     """xxx"""
     nbo = _get_notebook(notebook, library, index, force_reload=force_reload)
 
     nbo["code"] = nbo["temp"].replace("ipynb", "py")
@@ -306,15 +325,14 @@
     notebooks:
         dm.execute_notebook('basic',params={"EIN":"987654321"})
         npa = dm.import_notebook('npanalytics') # public nonprofit analytics
         dpa = dm.import_notebook('dpanalytics') # donorperfect analytics
     libraries: 
         dm.set_library("aimee")
         dm.set_library("benevolent")
-        dm.set_library("feltabout")
     """
     #
     print("datamachine https://pypi.org/project/datamachine/\n")
     idx = import_notebook(CURRENT["index"])
     print("idx: " + idx.INDEX + " " + CURRENT["index"])
     if "https:" in CURRENT["library"]:  # direct
         lib = import_notebook(CURRENT["library"])
```

### Comparing `datamachine-0.0.7/src/datamachine/xxx.py` & `datamachine-0.0.8/src/datamachine/xxx.py`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.7/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.0.8/src/datamachine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.7
+Version: 0.0.8
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="left">
+<p align="left" style="width: 20%; max-width: 240px; min-width: 80px;" >
   <img src="https://storage.googleapis.com/benevolent-machines/bm.svg" 
-       style="width: 20%; max-width: 240px; min-width: 80px;" 
        title="BenevolentMachines.Org">
 </p>
 
 # datamachine 
 
 ## Welcome to the Machine!
```


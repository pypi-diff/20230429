# Comparing `tmp/datamachine-0.0.8.tar.gz` & `tmp/datamachine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.8.tar", last modified: Sat Apr 29 02:42:23 2023, max compression
+gzip compressed data, was "datamachine-0.0.9.tar", last modified: Sat Apr 29 19:28:04 2023, max compression
```

## Comparing `datamachine-0.0.8.tar` & `datamachine-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.856263 datamachine-0.0.8/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3515 2023-04-29 02:42:23.856263 datamachine-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3033 2023-04-29 02:40:44.000000 datamachine-0.0.8/README.md
--rw-rw-rw-   0        0        0      520 2023-04-29 02:41:53.000000 datamachine-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      599 2023-04-29 02:42:23.857470 datamachine-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.834691 datamachine-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.840592 datamachine-0.0.8/src/datamachine/
--rw-rw-rw-   0        0        0      271 2023-04-29 02:02:57.000000 datamachine-0.0.8/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0    11385 2023-04-29 02:39:59.000000 datamachine-0.0.8/src/datamachine/_modular.py
--rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.8/src/datamachine/xxx.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:42:23.855342 datamachine-0.0.8/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0     3515 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 02:42:23.000000 datamachine-0.0.8/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 19:28:04.258594 datamachine-0.0.9/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3808 2023-04-29 19:28:04.259554 datamachine-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3356 2023-04-29 19:18:13.000000 datamachine-0.0.9/README.md
+-rw-rw-rw-   0        0        0      490 2023-04-29 19:27:30.000000 datamachine-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      599 2023-04-29 19:28:04.261349 datamachine-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 19:28:04.216820 datamachine-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 19:28:04.237651 datamachine-0.0.9/src/datamachine/
+-rw-rw-rw-   0        0        0      271 2023-04-29 02:02:57.000000 datamachine-0.0.9/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0    11257 2023-04-29 17:39:51.000000 datamachine-0.0.9/src/datamachine/_modular.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:28:04.257509 datamachine-0.0.9/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0     3808 2023-04-29 19:28:04.000000 datamachine-0.0.9/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-29 19:28:04.000000 datamachine-0.0.9/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 19:28:04.000000 datamachine-0.0.9/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 19:28:04.000000 datamachine-0.0.9/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.8/LICENSE` & `datamachine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.8/PKG-INFO` & `datamachine-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.8
-Summary: A data machine made of modular Python notebooks
+Version: 0.0.9
+Summary: Modular Notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="left" style="width: 20%; max-width: 240px; min-width: 80px;" >
-  <img src="https://storage.googleapis.com/benevolent-machines/bm.svg" 
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/datamachine2.svg" 
        title="BenevolentMachines.Org">
 </p>
 
-# datamachine 
-
 ## Welcome to the Machine!
 
-datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of libraries to their links. An index is a collection of libraries that is also stored in a JSON file.
+datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of notebooks to their links. 
 
 ## Features
 
 - Execute cloud notebooks with parameters: With datamachine, you can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
 
 - Import cloud notebooks as modules: Importing cloud notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
 
@@ -43,29 +41,36 @@
 
 ## Usage
 
 Once you have installed datamachine, you can use it to execute and import notebooks.
 
 ### Executing a Notebook
 
-To execute a notebook, use the `execute_notebook` function:
+To execute a notebook with parameters, use the `execute_notebook` function:
 
 ```python
 import datamachine as dm
-
 dm.execute_notebook(
-    "execute.ipynb", 
-    params={
-        "EIN": "343434343"
-    },
-    html="output.html",
+    "execute.ipynb", html="output.html",
+    params={"EIN": "200549531","TYPE": "summary"},
 )
 ```
 
-This command executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` set to `"343434343"`. The output is saved in an HTML file named `"output.html"`.
+This function executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` 
+set to `"200549531"`. The output is saved in an HTML file named `"output.html"`.
+
+In order to receive the EIN parameter in the executed notebook, simply invoke 
+the `execute_params` function with a passed dictionary containing the parameter.
+This function provides the test values when you're directly running the notebook, 
+and uses the passed values when invoked via `execute_notebook`.    
+```python
+import datamachine as dm
+params = dm.execute_params({"EIN": "454547709","TYPE": "detail"})
+EIN = params["EIN"]
+```
 
 ### Importing a Notebook as a Module
 
 To import a notebook as a module, use the `import_notebook` function:
 
 ```python
 import datamachine as dm
```

### Comparing `datamachine-0.0.8/README.md` & `datamachine-0.0.9/src/datamachine.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,29 @@
-<p align="left" style="width: 20%; max-width: 240px; min-width: 80px;" >
-  <img src="https://storage.googleapis.com/benevolent-machines/bm.svg" 
+Metadata-Version: 2.1
+Name: datamachine
+Version: 0.0.9
+Summary: Modular Notebooks
+Home-page: https://pypi.org/project/datamachine
+Author: Dave Killough
+Author-email: Dave Killough <dave.killough@gmail.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="left" >
+  <img src="https://storage.googleapis.com/benevolentmachines/datamachine2.svg" 
        title="BenevolentMachines.Org">
 </p>
 
-# datamachine 
-
 ## Welcome to the Machine!
 
-datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of libraries to their links. An index is a collection of libraries that is also stored in a JSON file.
+datamachine is a powerful Python package that allows you to execute cloud Python notebooks with parameters and import cloud notebooks as modules. With datamachine, you can reference notebooks from various sources such as local files, Colab links, Github links, and HTTP links, and execute or import them with ease. You can also assign codes to files or links and store them in a library, which is a collection of codes and their corresponding links. Libraries are stored in JSON format with a dictionary of notebooks to their links. 
 
 ## Features
 
 - Execute cloud notebooks with parameters: With datamachine, you can execute cloud notebooks with parameters, which is particularly useful when you want to run a notebook multiple times with different inputs.
 
 - Import cloud notebooks as modules: Importing cloud notebooks as modules is a breeze with datamachine. You can import notebooks from various sources such as local files, Colab links, Github links, and HTTP links.
 
@@ -29,29 +41,36 @@
 
 ## Usage
 
 Once you have installed datamachine, you can use it to execute and import notebooks.
 
 ### Executing a Notebook
 
-To execute a notebook, use the `execute_notebook` function:
+To execute a notebook with parameters, use the `execute_notebook` function:
 
 ```python
 import datamachine as dm
-
 dm.execute_notebook(
-    "execute.ipynb", 
-    params={
-        "EIN": "343434343"
-    },
-    html="output.html",
+    "execute.ipynb", html="output.html",
+    params={"EIN": "200549531","TYPE": "summary"},
 )
 ```
 
-This command executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` set to `"343434343"`. The output is saved in an HTML file named `"output.html"`.
+This function executes the notebook located at `"execute.ipynb"` with the parameter `"EIN"` 
+set to `"200549531"`. The output is saved in an HTML file named `"output.html"`.
+
+In order to receive the EIN parameter in the executed notebook, simply invoke 
+the `execute_params` function with a passed dictionary containing the parameter.
+This function provides the test values when you're directly running the notebook, 
+and uses the passed values when invoked via `execute_notebook`.    
+```python
+import datamachine as dm
+params = dm.execute_params({"EIN": "454547709","TYPE": "detail"})
+EIN = params["EIN"]
+```
 
 ### Importing a Notebook as a Module
 
 To import a notebook as a module, use the `import_notebook` function:
 
 ```python
 import datamachine as dm
```

### Comparing `datamachine-0.0.8/setup.cfg` & `datamachine-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 390d  version = 0.0.9.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
```

### Comparing `datamachine-0.0.8/src/datamachine/_modular.py` & `datamachine-0.0.9/src/datamachine/_modular.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,29 @@
             pid = temp_file.split("_")[1]
             if pid not in pids:
                 os.remove(temp_file)
 
     if "temp" not in notebook:  # new entry
         number = CURRENT["number"] = CURRENT["number"] + 1
         file_name = f"d_{CURRENT['process']}_{str(number)}.ipynb"
-        notebook["temp"] = f"{CURRENT['folder']}{os.path.sep}{file_name}"
+        file_name = f"{CURRENT['folder']}{os.path.sep}{file_name}"
+        notebook["temp"] = file_name
 
     if notebook["pull"].lower().startswith("https:"):
         with urlopen(notebook["pull"]) as in_url:
             with open(notebook["temp"], "wb") as out_file:
                 shutil.copyfileobj(in_url, out_file)
 
     else:  # it's a file!
         with open(notebook["pull"], encoding="utf-8") as in_file:
             with open(notebook["temp"], "w", encoding="utf-8") as out_file:
                 out_file.write(in_file.read())
 
 
-def _get_notebook(path, library=None, index=None, force_reload=False):
+def _get_notebook(path, library=None, force_reload=False):
 
     notebook = {}
 
     # check for a cached entry
     for item in CURRENT["notebooks"]:
         if item["path"] == path:
             notebook = item
@@ -93,20 +94,21 @@
         notebook["pull"] = path
 
     elif path.endswith(".ipynb"):
         notebook["pull"] = path
 
     else:  # assume we are left with a library and index to search
 
-        return _lookup_notebook(path, library, index)
+        return _lookup_notebook(path, library)
 
     _cache_notebook(notebook)
 
     if "path" in notebook:
         notebook["cached"] = True  # already imported
+
     else:  # new entry
         notebook["cached"] = False  # not yet imported
         notebook["path"] = path
         CURRENT["notebooks"].append(notebook)
 
     return notebook
 
@@ -160,74 +162,71 @@
     code = """
 ##############################################################################
 # Module file generated by datamachine. Any changes here will be lost.       #
 ##############################################################################
 """
     for cell in notebook_object["cells"]:
         if cell["cell_type"] == "code":
-            # transform the input to executable Python
             src = cell["source"]
             if src[0].startswith("#run"):
                 code += "\n# " + "# ".join(cell["source"])
             elif src[0].startswith("#test"):
                 code += "\n# " + "# ".join(cell["source"])
             else:
                 code += "".join(cell["source"])
         if cell["cell_type"] == "markdown":
             code += "\n# " + "# ".join(cell["source"])
         code += "\n\n"
     return code
 
 
-def _lookup_notebook(path, library, index):
+def _lookup_notebook(path, library):
     if library is None:
         library = CURRENT["library"]
     if ":" in library or "." in library:  # direct to library
         library_path = library
     else:  # lookup library in index
-        if index is None:
-            index = CURRENT["index"]
+        index = CURRENT["index"]
         idx = import_notebook(index)
         library_path = idx.LIBRARIES[library]["path"]
     lib = import_notebook(library_path)
     return _cache_notebook(lib.NOTEBOOKS[path]["path"])
 
 
 def _trace(line):
     if CURRENT["trace"] is True:
         path = f"{CURRENT['folder']}{os.path.sep}d_{CURRENT['process']}_trace.txt"
-        print(path)
         time_stamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S  ")
         with open(path, "a+", encoding="utf-8") as file_out:
             file_out.write(time_stamp + line + "\n")
 
 
 def _trace_off():
     CURRENT["trace"] = False
 
 
 def _trace_on():
     CURRENT["trace"] = True
 
 
 def execute_notebook(
-    notebook=None, library=None, index=None, html=None, params=None, force_reload=False,
+    notebook=None, library=None, html=None, params=None, force_reload=False,
 ):
     """Execute a notebook"""
 
     if not os.path.exists(CURRENT["folder"]):
         os.makedirs(CURRENT["folder"])
 
     _trace("execute_notebook('" + str(notebook) + "')")
-    nbo = _get_notebook(notebook, library, index, force_reload=force_reload)
+    nbo = _get_notebook(notebook, library, force_reload=force_reload)
 
     request = {  # pass to the executed notebook
         "notebook": notebook,
         "library": library,
-        "index": index,
+        "index": CURRENT["index"],
         "html": html,
         "params": params,
     }
 
     path = f"{CURRENT['folder']}{os.path.sep}d_{CURRENT['process']}_execute.json"
     with open(path, "w", encoding="utf-8") as file_out:
         json.dump(request, file_out, indent=4)
@@ -272,18 +271,18 @@
     with open(path, encoding="utf-8") as file_in:
         request = file_in.read()
         req = json.loads(request)
         return req["params"]
 
 
 def import_notebook(
-    notebook=None, library=None, index=None, force_reload=False,
+    notebook=None, library=None, force_reload=False,
 ):
     """xxx"""
-    nbo = _get_notebook(notebook, library, index, force_reload=force_reload)
+    nbo = _get_notebook(notebook, library, force_reload=force_reload)
 
     nbo["code"] = nbo["temp"].replace("ipynb", "py")
     with open(nbo["temp"], encoding="utf-8") as file_in:
         nbj = json.load(file_in)
         with open(nbo["code"], "w", encoding="utf-8") as code_file:
             code_file.write(_extract_code(nbj))
     nbo["module"] = nbo["code"].replace(".py", "").replace(os.path.sep, ".")
```


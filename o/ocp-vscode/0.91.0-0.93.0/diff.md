# Comparing `tmp/ocp_vscode-0.91.0.tar.gz` & `tmp/ocp_vscode-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-0.91.0.tar", last modified: Sun Apr 23 16:11:00 2023, max compression
+gzip compressed data, was "ocp_vscode-0.93.0.tar", last modified: Sat Apr 29 10:16:34 2023, max compression
```

## Comparing `ocp_vscode-0.91.0.tar` & `ocp_vscode-0.93.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.322681 ocp_vscode-0.91.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-0.91.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-23 16:11:00.322735 ocp_vscode-0.91.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     7866 2023-04-23 12:18:09.000000 ocp_vscode-0.91.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.321864 ocp_vscode-0.91.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      871 2023-04-16 10:39:54.000000 ocp_vscode-0.91.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-0.91.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9445 2023-04-22 08:41:23.000000 ocp_vscode-0.91.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    17668 2023-04-22 14:45:29.000000 ocp_vscode-0.91.0/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.322595 ocp_vscode-0.91.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      325 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      901 2023-04-23 16:11:00.322997 ocp_vscode-0.91.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1137 2023-04-23 12:18:09.000000 ocp_vscode-0.91.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079846 ocp_vscode-0.93.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-0.93.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-29 10:16:34.079907 ocp_vscode-0.93.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     7866 2023-04-29 07:30:35.000000 ocp_vscode-0.93.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079139 ocp_vscode-0.93.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      948 2023-04-27 17:11:08.000000 ocp_vscode-0.93.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-0.93.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    16915 2023-04-29 09:55:32.000000 ocp_vscode-0.93.0/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     9463 2023-04-27 18:50:45.000000 ocp_vscode-0.93.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18993 2023-04-29 06:29:08.000000 ocp_vscode-0.93.0/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079759 ocp_vscode-0.93.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      346 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      901 2023-04-29 10:16:34.080172 ocp_vscode-0.93.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1137 2023-04-29 07:30:35.000000 ocp_vscode-0.93.0/setup.py
```

### Comparing `ocp_vscode-0.91.0/LICENSE` & `ocp_vscode-0.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.91.0/PKG-INFO` & `ocp_vscode-0.93.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 0.91.0
+Version: 0.93.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.91.0/README.md` & `ocp_vscode-0.93.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 -   A fairly recent version of VS Code, e.g. 1.76.0 or newer
 -   [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) installed in VS Code
 -   `pip` available in the Python enviroment that will be used for CAD development
 
 **Steps**:
 
--   Download [ocp-cad-viewer-0.91.0.vsix](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases/download/v0.91.0/ocp-cad-viewer-0.91.0.vsix)
+-   Download [ocp-cad-viewer-0.93.0.vsix](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases/download/v0.93.0/ocp-cad-viewer-0.93.0.vsix)
 -   Install it locally in VS Code (_Extensions -> "..." menu -> Install from VSIX..._)
 -   Use the OCP CAD Viewer sidebar to manage both OCP CAD Viewer and python libraries:
     -   Install ocp_vscode via the blue button in the welcome screen of the "Viewer Manager" or by pressing the green down-arrow in the "Library Manager" section of the OCP CAD Viewer sidebar
     -   Install needed CAD libraries by pressing the green down-arrow behind the library name in the "Library Manager" section of the OCP CAD Viewer sidebar
 
 ![Installation](screenshots/ocp_vscode-install.gif)
```

### Comparing `ocp_vscode-0.91.0/ocp_vscode/__init__.py` & `ocp_vscode-0.93.0/ocp_vscode/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,8 +27,9 @@
     set_defaults,
     reset_defaults,
     get_default,
     get_defaults,
     status,
     set_port,
 )
+from .colors import ColorMap, CM, get_colormap, set_colormap, unset_colormap
 from .animation import Animation
```

### Comparing `ocp_vscode-0.91.0/ocp_vscode/animation.py` & `ocp_vscode-0.93.0/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.91.0/ocp_vscode/config.py` & `ocp_vscode-0.93.0/ocp_vscode/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
             j = json.dumps(data)
 
         with Timer(timeit, "", "http send", 1):
             r = requests.post(f"{CMD_URL}:{port}", data=j)
 
     except Exception as ex:
         print("Cannot connect to viewer, is it running and the right port provided?")
+        print(ex)
         return
 
     if r.status_code != 201:
         print("Error", r.text)
 
 
 def set_viewer_config(
```

### Comparing `ocp_vscode-0.91.0/ocp_vscode/show.py` & `ocp_vscode-0.93.0/ocp_vscode/show.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     preset,
     get_changed_config,
     workspace_config,
     combined_config,
     get_default,
     send,
 )
+from .colors import *
 
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
 
 def _tessellate(
     *cad_objs, names=None, colors=None, alphas=None, progress=None, **kwargs
 ):
@@ -194,14 +195,27 @@
             self.levels = levels
 
     def update(self, mark="+"):
         if mark in self.levels:
             print(mark, end="", flush=True)
 
 
+def align_attrs(attr_list, length, default, tag, explode=True):
+    if attr_list is None:
+        return [None] * length if explode else None
+    elif len(attr_list) < length:
+        print(f"Too view {tag}, using defaults to fill")
+        return list(attr_list) + [default] * (length - len(attr_list))
+    elif len(attr_list) > length:
+        print(f"Too many {tag}, trimming to length {length}")
+        return attr_list[:length]
+    else:
+        return attr_list
+
+
 def show(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     port=None,
     progress="-+c",
@@ -287,15 +301,15 @@
 
     - Renderer
         deviation:         Shapes: Deviation from linear deflection value (default=0.1)
         angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
         edge_accuracy:     Edges: Precision of edge discretization (default: mesh quality / 100)
 
         default_color:     Default mesh color (default=(232, 176, 36))
-        default_edgecolor: Default mesh color (default=(128, 128, 128))
+        default_edgecolor: Default color of the edges of a mesh (default=(128, 128, 128))
         ambient_intensity  Intensity of ambient ligth (default=1.0)
         direct_intensity   Intensity of direct lights (default=0.12)
 
         render_edges:      Render edges  (default=True)
         render_normals:    Render normals (default=False)
         render_mates:      Render mates for MAssemblies (default=False)
         render_joints:     Render build123d joints (default=False)
@@ -306,31 +320,59 @@
     - Debug
         debug:             Show debug statements to the VS Code browser console (default=False)
         timeit:            Show timing information from level 0-3 (default=False)
     """
 
     timeit = preset("timeit", timeit)
 
-    if names is not None and len(names) != len(cad_objs):
-        raise ValueError("Length of cad objects and names need to be the same")
+    names = align_attrs(names, len(cad_objs), None, "names", explode=False)
 
-    if colors is not None and len(colors) != len(cad_objs):
-        raise ValueError("Length of cad objects and colors need to be the same")
+    # Handle colormaps
 
-    if alphas is not None and len(alphas) != len(cad_objs):
-        raise ValueError("Length of cad objects and alphas need to be the same")
+    if isinstance(colors, ColorMap):
+        colors = [next(colors) for _ in range(len(cad_objs))]
+        alphas = [None] * len(cad_objs)  # alpha is encoded in colors
+    else:
+        colors = align_attrs(colors, len(cad_objs), None, "colors")
+        alphas = align_attrs(alphas, len(cad_objs), None, "alphas")
+
+    map_colors = None
+    colormap = get_colormap()
+    if colormap is not None:
+        map_colors = [next(colormap) for _ in range(len(cad_objs))]
+
+    for i in range(len(cad_objs)):
+        if isinstance(colors[i], str):
+            colors[i] = web_to_rgb(colors[i])
+        if colors[i] is None and map_colors is not None:
+            colors[i] = map_colors[i][:3]
+            if alphas[i] is None and len(map_colors[i]) == 4:
+                alphas[i] = map_colors[i][3]
+        elif colors[i] is not None:
+            if alphas[i] is None and len(colors[i]) == 4:
+                alphas[i] = colors[i][3]
+            colors[i] = colors[i][:3]
 
     if default_edgecolor is not None:
         default_edgecolor = Color(default_edgecolor).web_color
 
     kwargs = {
         k: v
         for k, v in locals().items()
         if v is not None
-        and k not in ["cad_objs", "names", "colors", "alphas", "port", "progress"]
+        and k
+        not in [
+            "cad_objs",
+            "names",
+            "colormap",
+            "colors",
+            "alphas",
+            "port",
+            "progress",
+        ]
     }
 
     progress = Progress([] if progress is None else [c for c in progress])
 
     with Timer(timeit, "", "overall"):
         data = _convert(
             *cad_objs,
@@ -445,15 +487,15 @@
 
     - Renderer
         deviation:         Shapes: Deviation from linear deflection value (default=0.1)
         angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
         edge_accuracy:     Edges: Precision of edge discretization (default: mesh quality / 100)
 
         default_color:     Default mesh color (default=(232, 176, 36))
-        default_edgecolor: Default mesh color (default=(128, 128, 128))
+        default_edgecolor: Default color of the edges of a mesh (default=(128, 128, 128))
         ambient_intensity  Intensity of ambient ligth (default=1.0)
         direct_intensity   Intensity of direct lights (default=0.12)
 
         render_edges:      Render edges  (default=True)
         render_normals:    Render normals (default=False)
         render_mates:      Render mates for MAssemblies (default=False)
         render_joints:     Render build123d joints (default=False)
@@ -477,32 +519,33 @@
 
     if clear:
         reset_show()
 
     if parent is not None:
         OBJECTS["objs"].append(parent)
         OBJECTS["names"].append("parent")
-        OBJECTS["colors"].append(get_default("default_color"))
-        OBJECTS["alphas"].append(0.25)
+        OBJECTS["colors"].append(None)
+        OBJECTS["alphas"].append(None)
 
+    color = None
+    alpha = None
     if options is None:
-        color = None
-        alpha = 1.0
+        colormap = get_colormap()
+        if colormap is not None:
+            for _ in range(len(OBJECTS["names"]) + 1):
+                *color, alpha = next(colormap)
     else:
         color = options.get("color")
         alpha = options.get("alpha", 1.0)
 
     OBJECTS["objs"].append(obj)
     OBJECTS["names"].append(name)
     OBJECTS["colors"].append(color)
     OBJECTS["alphas"].append(alpha)
 
-    # prefix = f"{name} " if name is not None else ""
-
-    # print(f"\nshow_object {prefix}<{obj}>")
     show(
         *OBJECTS["objs"],
         names=OBJECTS["names"],
         colors=OBJECTS["colors"],
         alphas=OBJECTS["alphas"],
         port=port,
         progress=progress,
```

### Comparing `ocp_vscode-0.91.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-0.93.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 0.91.0
+Version: 0.93.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.91.0/setup.cfg` & `ocp_vscode-0.93.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.91.0
+current_version = 0.93.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-0.91.0/setup.py` & `ocp_vscode-0.93.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "0.91.0",
+    "version": "0.93.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
-    "install_requires": ["ocp-tessellate>=1.0.0", "requests", "orjson"],
+    "install_requires": ["ocp-tessellate>=1.0.2", "requests", "orjson"],
     "packages": find_packages(),
     "zip_safe": False,
     "author": "Bernhard Walter",
     "author_email": "b_walter@arcor.de",
     "url": "https://github.com/bernhard-42/vscode-ocp-cad-viewer",
     "keywords": ["vscode", "widgets", "CAD", "cadquery"],
     "classifiers": [
```


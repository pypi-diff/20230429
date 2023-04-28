# Comparing `tmp/napari-SAM4IS-0.0.2.tar.gz` & `tmp/napari-SAM4IS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-SAM4IS-0.0.2.tar", last modified: Fri Apr 28 12:56:00 2023, max compression
+gzip compressed data, was "napari-SAM4IS-0.0.3.tar", last modified: Fri Apr 28 22:37:29 2023, max compression
```

## Comparing `napari-SAM4IS-0.0.2.tar` & `napari-SAM4IS-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 12:56:00.892420 napari-SAM4IS-0.0.2/
--rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/LICENSE
--rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/MANIFEST.in
--rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 12:56:00.892500 napari-SAM4IS-0.0.2/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     2700 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/README.md
--rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/pyproject.toml
--rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-04-28 12:56:00.892836 napari-SAM4IS-0.0.2/setup.cfg
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 12:56:00.889084 napari-SAM4IS-0.0.2/src/
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 12:56:00.890705 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/
--rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/SOURCES.txt
--rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/dependency_links.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/entry_points.txt
--rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/requires.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-04-28 12:56:00.000000 napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/top_level.txt
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 12:56:00.891852 napari-SAM4IS-0.0.2/src/napari_sam4is/
--rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-04-28 12:55:36.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/__init__.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 12:56:00.892198 napari-SAM4IS-0.0.2/src/napari_sam4is/_tests/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/_tests/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/_tests/test_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4660 2023-04-28 05:37:46.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/_utils.py
--rw-r--r--   0 hiroki     (501) staff       (20)    12017 2023-04-28 06:18:05.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.2/src/napari_sam4is/napari.yaml
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242872 napari-SAM4IS-0.0.3/
+-rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/LICENSE
+-rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/MANIFEST.in
+-rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 22:37:29.242940 napari-SAM4IS-0.0.3/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     2700 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/README.md
+-rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/pyproject.toml
+-rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-04-28 22:37:29.243270 napari-SAM4IS-0.0.3/setup.cfg
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.239608 napari-SAM4IS-0.0.3/src/
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.241261 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/
+-rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/entry_points.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/requires.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/top_level.txt
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242298 napari-SAM4IS-0.0.3/src/napari_sam4is/
+-rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-04-28 22:37:12.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/__init__.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242650 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/test_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4660 2023-04-28 05:37:46.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_utils.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    12040 2023-04-28 22:36:38.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/napari.yaml
```

### Comparing `napari-SAM4IS-0.0.2/LICENSE` & `napari-SAM4IS-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/PKG-INFO` & `napari-SAM4IS-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SAM4IS
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create annotations for instance segmentation using Segment Anything models
 Home-page: https://github.com/hiroalchem/napari-SAM4IS
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/hiroalchem/napari-SAM4IS/issues
 Project-URL: Documentation, https://github.com/hiroalchem/napari-SAM4IS#README.md
```

### Comparing `napari-SAM4IS-0.0.2/README.md` & `napari-SAM4IS-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/pyproject.toml` & `napari-SAM4IS-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/setup.cfg` & `napari-SAM4IS-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/src/napari_SAM4IS.egg-info/PKG-INFO` & `napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SAM4IS
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create annotations for instance segmentation using Segment Anything models
 Home-page: https://github.com/hiroalchem/napari-SAM4IS
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/hiroalchem/napari-SAM4IS/issues
 Project-URL: Documentation, https://github.com/hiroalchem/napari-SAM4IS#README.md
```

### Comparing `napari-SAM4IS-0.0.2/src/napari_sam4is/_tests/test_widget.py` & `napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/src/napari_sam4is/_utils.py` & `napari-SAM4IS-0.0.3/src/napari_sam4is/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.2/src/napari_sam4is/_widget.py` & `napari-SAM4IS-0.0.3/src/napari_sam4is/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,19 @@
         self._labels_layer_selection.addItems([layer.name for layer in self._viewer.layers if isinstance(layer, napari.layers.labels.labels.Labels)])
         self.vbox.addWidget(self._labels_layer_selection)
 
         self.vbox.addWidget(QLabel("Save as coco format \nin the same directory \nwith the input image"))
         self._save_btn = QPushButton("save")
         self._save_btn.clicked.connect(self._save)
         self.vbox.addWidget(self._save_btn)
-
+        """
         self._test_btn = QPushButton("corner")
         self._test_btn.clicked.connect(self.print_corner_value)
         self.vbox.addWidget(self._test_btn)
+        """
 
         self._sam_box_layer = self._viewer.add_shapes(name="SAM-Box", edge_color="red", edge_width=2, face_color="transparent")
         self._sam_box_layer.mouse_drag_callbacks.append(self._on_sam_box_created)
         self.lock_controls(self._sam_box_layer)
 
         if self._image_layer_selection.currentText() != "":
             self._image_type = check_image_type(self._viewer, self._image_layer_selection.currentText())
```


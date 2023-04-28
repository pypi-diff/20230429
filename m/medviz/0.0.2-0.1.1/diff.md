# Comparing `tmp/medviz-0.0.2.tar.gz` & `tmp/medviz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.0.2.tar", last modified: Wed Apr 19 15:21:26 2023, max compression
+gzip compressed data, was "medviz-0.1.1.tar", last modified: Fri Apr 28 23:21:09 2023, max compression
```

## Comparing `medviz-0.0.2.tar` & `medviz-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.0.2/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       26 2023-02-17 19:26:43.000000 medviz-0.0.2/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1471 2023-04-19 15:21:26.911847 medviz-0.0.2/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1000 2023-04-19 15:21:07.000000 medviz-0.0.2/README.rst
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       27 2023-04-19 14:27:12.000000 medviz-0.0.2/medviz/__init__.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1449 2023-04-19 00:22:28.000000 medviz-0.0.2/medviz/image_masks_axial.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1674 2023-04-19 14:44:02.000000 medviz-0.0.2/medviz/layered_plot.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-19 15:21:26.911847 medviz-0.0.2/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1471 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      273 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       93 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-04-19 15:21:26.000000 medviz-0.0.2/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      987 2023-04-19 15:10:51.000000 medviz-0.0.2/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-04-19 15:21:26.911847 medviz-0.0.2/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.0.2/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.1.1/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       26 2023-02-17 19:26:43.000000 medviz-0.1.1/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-04-28 23:21:09.994586 medviz-0.1.1/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.1.1/README.rst
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/medviz/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       47 2023-04-28 23:06:17.000000 medviz-0.1.1/medviz/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1160 2023-04-28 23:00:59.000000 medviz-0.1.1/medviz/example.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2049 2023-04-27 15:48:58.000000 medviz-0.1.1/medviz/gif.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2022 2023-04-28 22:56:59.000000 medviz-0.1.1/medviz/layered_plot.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/medviz.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      277 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      108 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/top_level.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1015 2023-04-28 23:20:56.000000 medviz-0.1.1/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-04-28 23:21:09.994586 medviz-0.1.1/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.1.1/setup.py
```

### Comparing `medviz-0.0.2/LICENSE` & `medviz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-0.0.2/PKG-INFO` & `medviz-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.0.2
+Version: 0.1.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -38,8 +38,31 @@
     import medviz
 
     medviz.layered_plot(image_path="dataset/1-1.nii", mask_paths=["dataset/small_bowel.nii", "dataset/1-1-label.nii"], mask_colors=["red", "yellow"], title="Layered Plot")
 
 The `layered_plot` function creates a layered plot of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting plot can be used to visualize the location of structures or regions of interest in the image.
 
 
+.. code-block:: python
+
+    import medviz
+
+    medviz.gif(
+        image_path="dataset/1-1.nii",
+        mask_paths=[
+            "dataset/small_bowel.nii",
+            "dataset/1-1-label.nii",
+            "dataset/vertebrae_L3.nii.gz",
+            "dataset/vertebrae_L4.nii.gz",
+            "dataset/vertebrae_L5.nii.gz",
+        ],
+        mask_colors=["red", "yellow", "green", "blue", "purple"],
+        title="Expert Annotations",
+        interval=70,
+        start_slice=30,
+        end_slice=130,
+        save_path="animation.gif",
+    )
+
+The `gif` function creates an animated GIF of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting GIF can be used to visualize the location of structures or regions of interest in the image.
+
 GitHub repository: [https://github.com/mohsenhariri/medviz](https://github.com/mohsenhariri/medviz)
```

### Comparing `medviz-0.0.2/README.rst` & `medviz-0.1.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -24,8 +24,31 @@
     import medviz
 
     medviz.layered_plot(image_path="dataset/1-1.nii", mask_paths=["dataset/small_bowel.nii", "dataset/1-1-label.nii"], mask_colors=["red", "yellow"], title="Layered Plot")
 
 The `layered_plot` function creates a layered plot of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting plot can be used to visualize the location of structures or regions of interest in the image.
 
 
+.. code-block:: python
+
+    import medviz
+
+    medviz.gif(
+        image_path="dataset/1-1.nii",
+        mask_paths=[
+            "dataset/small_bowel.nii",
+            "dataset/1-1-label.nii",
+            "dataset/vertebrae_L3.nii.gz",
+            "dataset/vertebrae_L4.nii.gz",
+            "dataset/vertebrae_L5.nii.gz",
+        ],
+        mask_colors=["red", "yellow", "green", "blue", "purple"],
+        title="Expert Annotations",
+        interval=70,
+        start_slice=30,
+        end_slice=130,
+        save_path="animation.gif",
+    )
+
+The `gif` function creates an animated GIF of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting GIF can be used to visualize the location of structures or regions of interest in the image.
+
 GitHub repository: [https://github.com/mohsenhariri/medviz](https://github.com/mohsenhariri/medviz)
```

### Comparing `medviz-0.0.2/medviz/layered_plot.py` & `medviz-0.1.1/medviz/layered_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,76 @@
+## Docstring: Layered plot of CT image and mask
+"""
+
+    Args:
+        image_path (str): Path to CT image
+        mask_paths (list): List of paths to masks
+        mask_colors (list): List of colors for masks
+        title (str): Title of plot
+
+    Returns:
+        None
+
+    Examples:
+        >>> import medviz
+        >>> medviz.layered_plot("data/ct.nii.gz", ["data/lung_mask.nii.gz", "data/heart_mask.nii.gz"], ["red", "yellow"], "Layered Plot")
+
+"""
 import numpy as np
 import nibabel as nib
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider
 
 
-
-
-
-def layered_plot(image_path, mask_paths, mask_colors=["red", "yellow"], title="Layered Plot"):
+def layered_plot(image_path, mask_paths, mask_colors, title="Layered Plot"):
     print("Loading images...")
-# Load the CT scan and mask imagesfsdf
-    ct_img = nib.load(image_path)
-    mask_img1 = nib.load(mask_paths[0])
-    mask_img2 = nib.load(mask_paths[1])
 
-    # Get the image data and mask data
+    ct_img = nib.load(image_path)
     ct_data = ct_img.get_fdata()
-    mask_data1 = mask_img1.get_fdata()
-    mask_data2 = mask_img2.get_fdata()
+    ct_data = np.flip(np.rot90(ct_data, axes=(1, 0)), axis=1)
 
-    # Rotate the images 90 degrees clockwise
-    ct_data = np.rot90(ct_data, axes=(1, 0))
-    mask_data1 = np.rot90(mask_data1, axes=(1, 0))
-    mask_data2 = np.rot90(mask_data2, axes=(1, 0))
+    mask_datas = []
+    for mask_path in mask_paths:
+        mask_data = nib.load(mask_path)
+        mask_data = np.flip(np.rot90(mask_data.get_fdata(), axes=(1, 0)), axis=1)
+        mask_datas.append(mask_data)
 
-    # Create a figure with a slider
-    fig, ax = plt.subplots()
+    _, ax = plt.subplots()
     plt.subplots_adjust(bottom=0.25)
-    ax.imshow(ct_data[:, :, ct_data.shape[2]//2], cmap='gray')
-    ax.contour(mask_data1[:, :, mask_data1.shape[2]//2], colors='r', levels=[0.5])
-    ax.contour(mask_data2[:, :, mask_data2.shape[2]//2], colors='b', levels=[0.5])
-    ax.set_xlabel('Slice Number')
+    ax.imshow(ct_data[:, :, ct_data.shape[2] // 2], cmap="gray")
+
+    for i in range(len(mask_datas)):
+        ax.contour(
+            mask_datas[i][:, :, mask_datas[i].shape[2] // 2],
+            colors=mask_colors[i],
+            levels=[0.5],
+        )
+
+    ax.set_xlabel("Slice Number")
+    ax.set_title(title)
+
     slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
-    slider = Slider(slider_ax, 'Slice', 0, ct_data.shape[2]-1, valinit=ct_data.shape[2]//2, valstep=1)
 
-    # Update the plot when the slider value changes
+    slider = Slider(
+        slider_ax,
+        "Slice",
+        0,
+        ct_data.shape[2] - 1,
+        valinit=ct_data.shape[2] // 2,
+        valstep=1,
+    )
+
     def update(val):
         slice_num = int(slider.val)
         ax.clear()
-        ax.imshow(ct_data[:, :, slice_num], cmap='gray')
-        ax.contour(mask_data1[:, :, slice_num], colors='r', levels=[0.5])
-        ax.contour(mask_data2[:, :, slice_num], colors='y', levels=[0.5])
-        ax.set_xlabel('Slice Number')
+        ax.imshow(ct_data[:, :, slice_num], cmap="gray")
+        for i in range(len(mask_datas)):
+            ax.contour(
+                mask_datas[i][:, :, slice_num], colors=mask_colors[i], levels=[0.5]
+            )
+
+        ax.set_xlabel("Slice Number")
+        ax.set_title(title)
 
     slider.on_changed(update)
+
     plt.show()
```

### Comparing `medviz-0.0.2/medviz.egg-info/PKG-INFO` & `medviz-0.1.1/medviz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.0.2
+Version: 0.1.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -38,8 +38,31 @@
     import medviz
 
     medviz.layered_plot(image_path="dataset/1-1.nii", mask_paths=["dataset/small_bowel.nii", "dataset/1-1-label.nii"], mask_colors=["red", "yellow"], title="Layered Plot")
 
 The `layered_plot` function creates a layered plot of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting plot can be used to visualize the location of structures or regions of interest in the image.
 
 
+.. code-block:: python
+
+    import medviz
+
+    medviz.gif(
+        image_path="dataset/1-1.nii",
+        mask_paths=[
+            "dataset/small_bowel.nii",
+            "dataset/1-1-label.nii",
+            "dataset/vertebrae_L3.nii.gz",
+            "dataset/vertebrae_L4.nii.gz",
+            "dataset/vertebrae_L5.nii.gz",
+        ],
+        mask_colors=["red", "yellow", "green", "blue", "purple"],
+        title="Expert Annotations",
+        interval=70,
+        start_slice=30,
+        end_slice=130,
+        save_path="animation.gif",
+    )
+
+The `gif` function creates an animated GIF of an image and one or more masks. The masks are overlaid on top of the image using the specified colors. The resulting GIF can be used to visualize the location of structures or regions of interest in the image.
+
 GitHub repository: [https://github.com/mohsenhariri/medviz](https://github.com/mohsenhariri/medviz)
```

### Comparing `medviz-0.0.2/pyproject.toml` & `medviz-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "medviz"
 authors = [{ name = "Mohsen Hariri", email = "mohsen.hariri@case.eud" }]
 description = "Medical Image Visualization Tool 🐍🚀🎉🦕"
-version = "0.0.2"
+version = "0.1.1"
 keywords = ["MRI", "CT"]
 license = { text = "GPL-3.0 License" }
 # https://github.com/pypi/warehouse/issues/869
 readme = "README.rst"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3.8",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   # "google-api-python-client==2.60.0",
   # "google-auth-oauthlib==0.5.2",
-  "numpy==1.21.2",
+  "numpy >= 1.19.5",
   'importlib-metadata; python_version<"3.8"',
-  "matplotlib==3.4.3",
-  "nibabel==3.2.1",
+  "matplotlib >= 3.3.4",
+  "nibabel >= 3.2.1",
+  "imageio >= 2.9.0",
 ]
 
 [tool.setuptools]
 packages = ["medviz"]
 
 [tool.isort]
 profile = "black"
```


# Comparing `tmp/napari-clusters-plotter-0.6.2.tar.gz` & `tmp/napari-clusters-plotter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-clusters-plotter-0.6.2.tar", last modified: Fri Mar 17 12:35:39 2023, max compression
+gzip compressed data, was "napari-clusters-plotter-0.7.0.tar", last modified: Sat Apr 29 18:02:12 2023, max compression
```

## Comparing `napari-clusters-plotter-0.6.2.tar` & `napari-clusters-plotter-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 12:35:39.485421 napari-clusters-plotter-0.6.2/
--rw-rw-rw-   0        0        0     1642 2022-12-08 10:19:42.000000 napari-clusters-plotter-0.6.2/LICENSE
--rw-rw-rw-   0        0        0      127 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0    19799 2023-03-17 12:35:39.485421 napari-clusters-plotter-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    18410 2023-02-13 14:36:39.000000 napari-clusters-plotter-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 12:35:39.373488 napari-clusters-plotter-0.6.2/napari_clusters_plotter/
--rw-rw-rw-   0        0        0    18027 2023-03-17 12:34:56.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_Qt_code.py
--rw-rw-rw-   0        0        0      184 2023-03-17 12:34:33.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/__init__.py
--rw-rw-rw-   0        0        0    21241 2023-03-17 12:32:50.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_clustering.py
--rw-rw-rw-   0        0        0    35126 2023-03-17 12:32:50.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_dimensionality_reduction.py
--rw-rw-rw-   0        0        0      406 2023-01-10 12:32:33.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_dock_widget.py
--rw-rw-rw-   0        0        0    21999 2023-03-17 12:34:56.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_plotter.py
--rw-rw-rw-   0        0        0    11054 2023-03-14 22:16:16.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_plotter_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:35:39.451562 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/
--rw-rw-rw-   0        0        0        0 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/__init__.py
--rw-rw-rw-   0        0        0     7838 2023-03-17 12:32:50.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_clustering.py
--rw-rw-rw-   0        0        0     7159 2023-03-14 22:16:16.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_dimension_reduction.py
--rw-rw-rw-   0        0        0     2457 2023-03-16 15:33:07.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_dock_widget.py
--rw-rw-rw-   0        0        0     4713 2023-03-13 13:04:15.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_plotter.py
--rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:07.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_utils.py
--rw-rw-rw-   0        0        0    15548 2023-03-17 12:32:50.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:35:39.482802 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/
--rw-rw-rw-   0        0        0     6680 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Back.png
--rw-rw-rw-   0        0        0     6951 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Customize.png
--rw-rw-rw-   0        0        0     6535 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Forward.png
--rw-rw-rw-   0        0        0     7143 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Home.png
--rw-rw-rw-   0        0        0     7114 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Pan.png
--rw-rw-rw-   0        0        0    11810 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Pan_checked.png
--rw-rw-rw-   0        0        0     7381 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Save.png
--rw-rw-rw-   0        0        0     6739 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Subplots.png
--rw-rw-rw-   0        0        0     8064 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Zoom.png
--rw-rw-rw-   0        0        0    12372 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Zoom_checked.png
-drwxrwxrwx   0        0        0        0 2023-03-17 12:35:39.404695 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/
--rw-rw-rw-   0        0        0    19799 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1384 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      149 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-03-17 12:35:39.000000 napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-03-17 12:32:50.000000 napari-clusters-plotter-0.6.2/requirements.txt
--rw-rw-rw-   0        0        0     1919 2023-03-17 12:35:39.485421 napari-clusters-plotter-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      117 2022-03-15 17:32:25.000000 napari-clusters-plotter-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.717066 napari-clusters-plotter-0.7.0/
+-rw-rw-rw-   0        0        0     1642 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15617 2023-04-29 18:02:12.717066 napari-clusters-plotter-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14228 2023-04-29 17:52:49.000000 napari-clusters-plotter-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.671663 napari-clusters-plotter-0.7.0/napari_clusters_plotter/
+-rw-rw-rw-   0        0        0    24305 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_Qt_code.py
+-rw-rw-rw-   0        0        0      184 2023-04-29 17:56:31.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/__init__.py
+-rw-rw-rw-   0        0        0    21295 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_clustering.py
+-rw-rw-rw-   0        0        0    37507 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dimensionality_reduction.py
+-rw-rw-rw-   0        0        0      406 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dock_widget.py
+-rw-rw-rw-   0        0        0    33249 2023-04-29 17:16:06.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter.py
+-rw-rw-rw-   0        0        0    17769 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.705752 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/
+-rw-rw-rw-   0        0        0        0 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/__init__.py
+-rw-rw-rw-   0        0        0     7838 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_clustering.py
+-rw-rw-rw-   0        0        0     7373 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dimension_reduction.py
+-rw-rw-rw-   0        0        0     2457 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dock_widget.py
+-rw-rw-rw-   0        0        0     6619 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_plotter.py
+-rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:04.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_utils.py
+-rw-rw-rw-   0        0        0    15576 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.716063 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/
+-rw-rw-rw-   0        0        0     6680 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Back.png
+-rw-rw-rw-   0        0        0     6951 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Customize.png
+-rw-rw-rw-   0        0        0     6535 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Forward.png
+-rw-rw-rw-   0        0        0     7143 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Home.png
+-rw-rw-rw-   0        0        0     7114 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan.png
+-rw-rw-rw-   0        0        0    11810 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan_checked.png
+-rw-rw-rw-   0        0        0     7381 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Save.png
+-rw-rw-rw-   0        0        0     6739 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Subplots.png
+-rw-rw-rw-   0        0        0     8064 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom.png
+-rw-rw-rw-   0        0        0    12372 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom_checked.png
+drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.699737 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/
+-rw-rw-rw-   0        0        0    15617 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1384 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/requirements.txt
+-rw-rw-rw-   0        0        0     1928 2023-04-29 18:02:12.719071 napari-clusters-plotter-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      117 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/setup.py
```

### Comparing `napari-clusters-plotter-0.6.2/LICENSE` & `napari-clusters-plotter-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/PKG-INFO` & `napari-clusters-plotter-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-clusters-plotter
-Version: 0.6.2
+Version: 0.7.0
 Summary: A plugin to use with napari for clustering objects according to their properties
 Home-page: https://github.com/BiAPoL/napari-clusters-plotter
 Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
 Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
@@ -28,30 +28,22 @@
 
 # napari-clusters-plotter
 
 [![License](https://img.shields.io/pypi/l/napari-clusters-plotter.svg?color=green)](https://github.com/lazigu/napari-clusters-plotter/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-clusters-plotter.svg?color=green)](https://pypi.org/project/napari-clusters-plotter)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-clusters-plotter.svg?color=green)](https://python.org)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/version.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
-[![tests](https://github.com/lazigu/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/lazigu/napari-clusters-plotter/actions)
+[![tests](https://github.com/BiAPoL/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/napari-clusters-plotter/actions)
 [![codecov](https://codecov.io/gh/BiAPoL/napari-clusters-plotter/branch/main/graph/badge.svg?token=R6W2KO1NJ8)](https://codecov.io/gh/BiAPoL/napari-clusters-plotter)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/downloads.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-clusters-plotter)](https://www.napari-hub.org/plugins/napari-clusters-plotter)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7011471.svg)](https://doi.org/10.5281/zenodo.7011471)
 
-A plugin to use with napari for clustering objects according to their properties.
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
-<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
-
-Demonstration of handling 3D time-lapse data:
+A napari-plugin for clustering objects according to their properties.
 
 <img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast2_timelapse.gif" width="700"/>
 
 ----------------------------------
 
 Jump to:
 - [Usage](#usage)
@@ -76,253 +68,176 @@
 For clustering objects according to their properties, the starting point is a [grey-value image](example_data/blobs.tif) and a label image
 representing a segmentation of objects. For segmenting objects, you can for example use the
 [Voronoi-Otsu-labelling approach](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#voronoi-otsu-labelling)
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
-### Measurements
-The first step is deriving measurements from the labelled image and the corresponding pixels in the grey-value image.
-Since the 0.6.0 release measurements widget is no longer part of this plugin and you will have to use other napari plugins to measure your data.
-One way is to use the measurement functions in [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops), which comes pre-installed with the napari cluster plotter.
-Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget.
-Just select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-In the previous napari-cluster-plotter release a GPU dependant measurement function was implemented which you can find in the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-To use this function you will need to install this library (see optional installation steps) and you can find the widget under the menu `Tools > Measurement tables > Label statistics (clEsperanto)`. As before, select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. Also, close the Measure widget.
-
-If you want to upload your own measurements you can do this using [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops).
-Under the menu `Tools > Measurement tables > Load from CSV (nsr)` you can find a widget to upload your own csv file.
-Make sure that there is a column that specifies the which measurement belongs to which label by adding a column with the name "label".
-If you don't specify this column it will be assumed that measurements start at 1 and each
-column describes the next label.
-
-Note that tables for time-lapse data need to include an **additional column named "frame"**, which indicates which slice in
-time the given row refers to.
-
-**For the correct visualisation of clusters IDs in space**, it is **important** that label images/time-points of the time-lapse
-are either **labelled sequentially** or missing labels still exist in the loaded csv file (i.e., missing label exists in the
-"label" column with `NaN` values for other measurements in the same row). If you perform measurements using before mentioned
-plugins, the obtained dataframe is already in the correct form.
-
-#### Time-Lapse Measurements
-In case you have 2D time-lapse data you need to convert it into a suitable shape using the function: `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)`,
-which can be found in the [napari time slicer](https://www.napari-hub.org/plugins/napari-time-slicer).
-
-Note that tables for time-lapse data will include an additional column named "frame", which indicates which slice in
-time the given row refers to. If you want to import your own csv files for time-lapse data make sure to include this column!
-If you have tracking data where each column specifies measurements for a track instead of a label at a specific time point,
-this column must not be added.
+In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
-Both [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops) and [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant) include measuring widgets for timelapse data.
+### Measurements
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
+Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
+A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+At this point it is recommended to close the table and the Measure widget to free space for following steps.
+
+You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
+If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
+Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
 
-Once measurements were made or uploaded, these measurements were saved in the `properties/features` of the labels layer which was
-analysed. You can then plot these measurements using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
+Once measurements were saved in the labels layer which was analysed, you can then plot these measurements using the menu `Tools > Visualization > Plot measurements (ncp)`.
 
 In this widget, you can select the labels layer which was analysed and the measurements which should be plotted
-on the X- and Y-axis. If you cannot see any options in axes selection boxes, but you have performed measurements, click
-on `Update Axes/Clustering Selection Boxes` to refresh them. Click on `Run` to draw the data points in the plot area.
+on the X- and Y-axis. Click on `Plot` to draw the data points in the plot area.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_plain.png)
 
-You can also manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
+Under advanced options, you can also select the plot type histogram which will visualize a 2D histogram. 2D histogram visualization is recommended if you have a very high number of data points.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_2d.png)
+
+If you choose the same measurement for the X and the Y axis, a histogram will be shown.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_1d.png)
+
+Under advanced options you will also find the checkbox determining whether not-selected data points should be hidden (shown in grey) or automatically
+clustered as another cluster.
+
+### Manual clustering
+
+You can manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
 rectangle - right click. The resulting manual clustering will also be visualized in the original image. To optimize
 visualization in the image, turn off the visibility of the analysed labels layer.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_interactive.png)
+<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
 
 Hold down the SHIFT key while annotating regions in the plot to manually select multiple clusters.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/multi-select-manual-clustering.gif)
 
-#### Time-Lapse Plotting
+### Saving manual clustering
+
+Manual clustering results can be saved by going to `Tools > Measurement > Show table (nsr)`, and clicking on `Save as csv`.
+The saved table will contain a "MANUAL_CLUSTER_ID" column. This column is overwritten every time different clusters are manually selected.
+
+### Time-Lapse analysis
+
 When you plot your time-lapse datasets you will notice that the plots look slightly different.
-Datapoints of the current time frame are highlighted in white and you can see the datapoints move through the plot if you press play:
+Datapoints of the current time frame are highlighted in bright color and you can see the datapoints move through the plot while you navigate through time:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plotting_time-lapse_data_as_movie.gif)
 
 You can also manually select groups using the lasso tool and plot a measurement per frame and see how the group behaves in time.
 Furthermore, you could also select a group in time and see where the datapoints lie in a different feature space:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/timelapse_manual_clustering_tips.gif)
 
-### Dimensionality reduction: UMAP, t-SNE or PCA
+If you have custom measurements from tracking data where each column specifies measurements for a track instead of a label at a specific time point, the `frame` column must not be added.
+
+### Dimensionality reduction
 
-For getting more insights into your data, you can reduce the dimensionality of the measurements, e.g.
-using the [UMAP algorithm](https://umap-learn.readthedocs.io/en/latest/), [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
-or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html).
-To apply it to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be
-dimensionality reduced. By default, all measurements are selected in the box. If you cannot see any measurements, but
-you have performed them, click on `Update Measurements` to refresh the box. You can read more about parameters of both
-algorithms by hovering over question marks or by clicking on them. When you are done with the selection, click on `Run`
-and after a moment, the table of measurements will re-appear with two additional columns representing the reduced
-dimensions of the dataset. These columns are automatically saved in the `properties` of the labels layer so there is no
-need to save them for usage in other widgets unless you wish to do so.
+For getting more insights into your data, you can reduce the dimensionality of the measurements, using these algorithms:
+* [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
+* [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
+* [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
+* [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
+* [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
+
+To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
+By default, all measurements are selected in the box. 
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
-Afterwards, you can again save and/or close the table. Also, close the Dimensionality Reduction widget.
+Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
-again, select the analysed labels layer.
-This time select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+select the analysed labels layer.
+Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
 
-Afterwards, you can again save and/or close the table. Also, close the clustering widget.
+Afterwards, you can save and/or close the table.
 
 ### Plotting clustering results
-Return to the Plotter widget using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
-Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Run`.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
+Return to the Plotter widget using the menu `Tools > Visualization > Plot measurement (ncp)`.
+Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Plot`.
 
-Example of k-means clustering results:
-
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/kmeans_clusters_plot.png)
+![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
 
 ## Installation
 ### Devbio-napari installation
-The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) library.
-This library installs napari alongside many other useful plugins, including the napari-clusters-plotter.
-We recommend this library as it is not only the easiest way to install the napari-cluster-plotter, but it includes plugins for segmentation and measurement, which we don't provide.
-There are detailed installation instructions on the [napari-hub-page](https://www.napari-hub.org/plugins/devbio-napari) if you have any problems installing it.
-In case you want to have a minimal installation of our plugin you can find other installation options below.
+
+The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
-  If you never used python/conda environments before, please follow the instructions
-  [here](https://mpicbg-scicomp.github.io/ipf_howtoguides/guides/Python_Conda_Environments) first. It is recommended to
-  install python 3.9 to your new conda environment from the start. The plugin is not yet supported with Python 3.10.
-  Create a new environment, for example, like this:
+  If you never used mamba/conda environments before, please follow the instructions
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
 
-```
-conda create --name ncp-env python=3.9
-```
-
-* Activate the new environment via conda:
-
-```
-conda activate ncp-env
-```
-
-* Install [napari], e.g. via [conda]:
+* Create a new environment, for example, like this:
 
 ```
-conda install -c conda-forge napari
+mamba create --name ncp-env python=3.9
 ```
 
-Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
-
-```
-conda install -c conda-forge napari-clusters-plotter
-```
-
-### Optional installation
-Follow these steps instead of the regular installation to include the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-Creating the environment like this will allow you to use your GPU to render your cluster results.
-Furthermore, you can access the deprecated measurement functions of the napari-cluster-plotter in releases < 0.6.0.
-If you have trouble with this library you can use the regular installation above.
-
-```
-conda create --name ncp-env python==3.9
-```
-
-
 * Activate the new environment via conda:
 
 ```
-conda activate ncp-env
+mamba activate ncp-env
 ```
 
-* Install napari-pyclesperanto-assistant, e.g. with pip:
-
-```
-pip install napari-pyclesperanto-assistant
-```
-
-* Mac-users please also install this:
-
-```
-conda install -c conda-forge ocl_icd_wrapper_apple
-```
-
-* Linux users please also install this:
-
-```
-conda install -c conda-forge ocl-icd-system
-```
-
-* Install [napari], e.g. via [pip] or [conda]:
+* Install [napari], e.g. via [conda]:
 
 ```
-python -m pip install "napari[all]"
-```
-```
-conda install -c conda-forge napari
+mamba install -c conda-forge napari
 ```
 
 Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
 
 ```
-conda install -c conda-forge napari-clusters-plotter
+mamba install -c conda-forge napari-clusters-plotter
 ```
 
 ## Troubleshooting installation
 
-- If the plugin does not appear in napari 'Plugins' menu, and in 'Plugin errors...' you can see such an error:
-
-```
-ImportError: DLL load failed while importing _cl
-```
-
-Try downloading and installing a pyopencl with a lower cl version, e.g. cl12 : pyopencl=2020.1. However, in this case,
-you will need an environment with a lower python version (python=3.8).
-
 - `Error: Could not build wheels for hdbscan which use PEP 517 and cannot be installed directly`
 
 This can happen if you used pip for the installation. To solve this error, install hdbscan via conda before installing the plugin:
 
 ```
-conda install -c conda-forge hdbscan
+mamba install -c conda-forge hdbscan
 ```
 
 - `ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 96 from C header, got 88 from PyObject`
 
 Similar to the above-described error, this error can occur when importing hdbscan through pip or in the wrong order. This can be fixed by installing packages separately through conda and in the following order:
 ```bash
-conda install -c conda-forge napari pyopencl hdbscan
+mamba install -c conda-forge napari hdbscan
 pip install napari-clusters-plotter
 ```
 
-- `WARNING: No ICDs were found` or `LogicError: clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR`
-
-Make your system-wide implementation visible by installing either of the following conda packages:
-
-```
-conda install -c conda-forge ocl-icd-system
-conda install -c conda-forge ocl_icd_wrapper_apple
-```
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [pytest], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-clusters-plotter-0.6.2/README.md` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,49 @@
+Metadata-Version: 2.1
+Name: napari-clusters-plotter
+Version: 0.7.0
+Summary: A plugin to use with napari for clustering objects according to their properties
+Home-page: https://github.com/BiAPoL/napari-clusters-plotter
+Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
+Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
+Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
+Project-URL: Source Code, https://github.com/BiAPoL/napari-clusters-plotter
+Project-URL: User Support, https://github.com/BiAPoL/napari-clusters-plotter/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Framework :: napari
+Classifier: Topic :: Software Development :: Testing
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # napari-clusters-plotter
 
 [![License](https://img.shields.io/pypi/l/napari-clusters-plotter.svg?color=green)](https://github.com/lazigu/napari-clusters-plotter/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-clusters-plotter.svg?color=green)](https://pypi.org/project/napari-clusters-plotter)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-clusters-plotter.svg?color=green)](https://python.org)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/version.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
-[![tests](https://github.com/lazigu/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/lazigu/napari-clusters-plotter/actions)
+[![tests](https://github.com/BiAPoL/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/napari-clusters-plotter/actions)
 [![codecov](https://codecov.io/gh/BiAPoL/napari-clusters-plotter/branch/main/graph/badge.svg?token=R6W2KO1NJ8)](https://codecov.io/gh/BiAPoL/napari-clusters-plotter)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/downloads.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-clusters-plotter)](https://www.napari-hub.org/plugins/napari-clusters-plotter)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7011471.svg)](https://doi.org/10.5281/zenodo.7011471)
 
-A plugin to use with napari for clustering objects according to their properties.
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
-<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
-
-Demonstration of handling 3D time-lapse data:
+A napari-plugin for clustering objects according to their properties.
 
 <img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast2_timelapse.gif" width="700"/>
 
 ----------------------------------
 
 Jump to:
 - [Usage](#usage)
@@ -48,253 +68,176 @@
 For clustering objects according to their properties, the starting point is a [grey-value image](example_data/blobs.tif) and a label image
 representing a segmentation of objects. For segmenting objects, you can for example use the
 [Voronoi-Otsu-labelling approach](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#voronoi-otsu-labelling)
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
-### Measurements
-The first step is deriving measurements from the labelled image and the corresponding pixels in the grey-value image.
-Since the 0.6.0 release measurements widget is no longer part of this plugin and you will have to use other napari plugins to measure your data.
-One way is to use the measurement functions in [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops), which comes pre-installed with the napari cluster plotter.
-Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget.
-Just select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-In the previous napari-cluster-plotter release a GPU dependant measurement function was implemented which you can find in the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-To use this function you will need to install this library (see optional installation steps) and you can find the widget under the menu `Tools > Measurement tables > Label statistics (clEsperanto)`. As before, select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. Also, close the Measure widget.
-
-If you want to upload your own measurements you can do this using [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops).
-Under the menu `Tools > Measurement tables > Load from CSV (nsr)` you can find a widget to upload your own csv file.
-Make sure that there is a column that specifies the which measurement belongs to which label by adding a column with the name "label".
-If you don't specify this column it will be assumed that measurements start at 1 and each
-column describes the next label.
-
-Note that tables for time-lapse data need to include an **additional column named "frame"**, which indicates which slice in
-time the given row refers to.
-
-**For the correct visualisation of clusters IDs in space**, it is **important** that label images/time-points of the time-lapse
-are either **labelled sequentially** or missing labels still exist in the loaded csv file (i.e., missing label exists in the
-"label" column with `NaN` values for other measurements in the same row). If you perform measurements using before mentioned
-plugins, the obtained dataframe is already in the correct form.
-
-#### Time-Lapse Measurements
-In case you have 2D time-lapse data you need to convert it into a suitable shape using the function: `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)`,
-which can be found in the [napari time slicer](https://www.napari-hub.org/plugins/napari-time-slicer).
-
-Note that tables for time-lapse data will include an additional column named "frame", which indicates which slice in
-time the given row refers to. If you want to import your own csv files for time-lapse data make sure to include this column!
-If you have tracking data where each column specifies measurements for a track instead of a label at a specific time point,
-this column must not be added.
+In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
-Both [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops) and [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant) include measuring widgets for timelapse data.
+### Measurements
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
+Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
+A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+At this point it is recommended to close the table and the Measure widget to free space for following steps.
+
+You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
+If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
+Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
 
-Once measurements were made or uploaded, these measurements were saved in the `properties/features` of the labels layer which was
-analysed. You can then plot these measurements using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
+Once measurements were saved in the labels layer which was analysed, you can then plot these measurements using the menu `Tools > Visualization > Plot measurements (ncp)`.
 
 In this widget, you can select the labels layer which was analysed and the measurements which should be plotted
-on the X- and Y-axis. If you cannot see any options in axes selection boxes, but you have performed measurements, click
-on `Update Axes/Clustering Selection Boxes` to refresh them. Click on `Run` to draw the data points in the plot area.
+on the X- and Y-axis. Click on `Plot` to draw the data points in the plot area.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_plain.png)
 
-You can also manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
+Under advanced options, you can also select the plot type histogram which will visualize a 2D histogram. 2D histogram visualization is recommended if you have a very high number of data points.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_2d.png)
+
+If you choose the same measurement for the X and the Y axis, a histogram will be shown.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_1d.png)
+
+Under advanced options you will also find the checkbox determining whether not-selected data points should be hidden (shown in grey) or automatically
+clustered as another cluster.
+
+### Manual clustering
+
+You can manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
 rectangle - right click. The resulting manual clustering will also be visualized in the original image. To optimize
 visualization in the image, turn off the visibility of the analysed labels layer.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_interactive.png)
+<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
 
 Hold down the SHIFT key while annotating regions in the plot to manually select multiple clusters.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/multi-select-manual-clustering.gif)
 
-#### Time-Lapse Plotting
+### Saving manual clustering
+
+Manual clustering results can be saved by going to `Tools > Measurement > Show table (nsr)`, and clicking on `Save as csv`.
+The saved table will contain a "MANUAL_CLUSTER_ID" column. This column is overwritten every time different clusters are manually selected.
+
+### Time-Lapse analysis
+
 When you plot your time-lapse datasets you will notice that the plots look slightly different.
-Datapoints of the current time frame are highlighted in white and you can see the datapoints move through the plot if you press play:
+Datapoints of the current time frame are highlighted in bright color and you can see the datapoints move through the plot while you navigate through time:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plotting_time-lapse_data_as_movie.gif)
 
 You can also manually select groups using the lasso tool and plot a measurement per frame and see how the group behaves in time.
 Furthermore, you could also select a group in time and see where the datapoints lie in a different feature space:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/timelapse_manual_clustering_tips.gif)
 
-### Dimensionality reduction: UMAP, t-SNE or PCA
+If you have custom measurements from tracking data where each column specifies measurements for a track instead of a label at a specific time point, the `frame` column must not be added.
+
+### Dimensionality reduction
 
-For getting more insights into your data, you can reduce the dimensionality of the measurements, e.g.
-using the [UMAP algorithm](https://umap-learn.readthedocs.io/en/latest/), [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
-or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html).
-To apply it to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be
-dimensionality reduced. By default, all measurements are selected in the box. If you cannot see any measurements, but
-you have performed them, click on `Update Measurements` to refresh the box. You can read more about parameters of both
-algorithms by hovering over question marks or by clicking on them. When you are done with the selection, click on `Run`
-and after a moment, the table of measurements will re-appear with two additional columns representing the reduced
-dimensions of the dataset. These columns are automatically saved in the `properties` of the labels layer so there is no
-need to save them for usage in other widgets unless you wish to do so.
+For getting more insights into your data, you can reduce the dimensionality of the measurements, using these algorithms:
+* [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
+* [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
+* [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
+* [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
+* [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
+
+To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
+By default, all measurements are selected in the box. 
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
-Afterwards, you can again save and/or close the table. Also, close the Dimensionality Reduction widget.
+Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
-again, select the analysed labels layer.
-This time select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+select the analysed labels layer.
+Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
 
-Afterwards, you can again save and/or close the table. Also, close the clustering widget.
+Afterwards, you can save and/or close the table.
 
 ### Plotting clustering results
-Return to the Plotter widget using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
-Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Run`.
-
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
 
-Example of k-means clustering results:
+Return to the Plotter widget using the menu `Tools > Visualization > Plot measurement (ncp)`.
+Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Plot`.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/kmeans_clusters_plot.png)
+![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
 
 ## Installation
 ### Devbio-napari installation
-The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) library.
-This library installs napari alongside many other useful plugins, including the napari-clusters-plotter.
-We recommend this library as it is not only the easiest way to install the napari-cluster-plotter, but it includes plugins for segmentation and measurement, which we don't provide.
-There are detailed installation instructions on the [napari-hub-page](https://www.napari-hub.org/plugins/devbio-napari) if you have any problems installing it.
-In case you want to have a minimal installation of our plugin you can find other installation options below.
+
+The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
-  If you never used python/conda environments before, please follow the instructions
-  [here](https://mpicbg-scicomp.github.io/ipf_howtoguides/guides/Python_Conda_Environments) first. It is recommended to
-  install python 3.9 to your new conda environment from the start. The plugin is not yet supported with Python 3.10.
-  Create a new environment, for example, like this:
-
-```
-conda create --name ncp-env python=3.9
-```
-
-* Activate the new environment via conda:
-
-```
-conda activate ncp-env
-```
-
-* Install [napari], e.g. via [conda]:
+  If you never used mamba/conda environments before, please follow the instructions
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
 
-```
-conda install -c conda-forge napari
-```
-
-Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
+* Create a new environment, for example, like this:
 
 ```
-conda install -c conda-forge napari-clusters-plotter
+mamba create --name ncp-env python=3.9
 ```
 
-### Optional installation
-Follow these steps instead of the regular installation to include the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-Creating the environment like this will allow you to use your GPU to render your cluster results.
-Furthermore, you can access the deprecated measurement functions of the napari-cluster-plotter in releases < 0.6.0.
-If you have trouble with this library you can use the regular installation above.
-
-```
-conda create --name ncp-env python==3.9
-```
-
-
 * Activate the new environment via conda:
 
 ```
-conda activate ncp-env
-```
-
-* Install napari-pyclesperanto-assistant, e.g. with pip:
-
-```
-pip install napari-pyclesperanto-assistant
-```
-
-* Mac-users please also install this:
-
-```
-conda install -c conda-forge ocl_icd_wrapper_apple
+mamba activate ncp-env
 ```
 
-* Linux users please also install this:
+* Install [napari], e.g. via [conda]:
 
 ```
-conda install -c conda-forge ocl-icd-system
-```
-
-* Install [napari], e.g. via [pip] or [conda]:
-
-```
-python -m pip install "napari[all]"
-```
-```
-conda install -c conda-forge napari
+mamba install -c conda-forge napari
 ```
 
 Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
 
 ```
-conda install -c conda-forge napari-clusters-plotter
+mamba install -c conda-forge napari-clusters-plotter
 ```
 
 ## Troubleshooting installation
 
-- If the plugin does not appear in napari 'Plugins' menu, and in 'Plugin errors...' you can see such an error:
-
-```
-ImportError: DLL load failed while importing _cl
-```
-
-Try downloading and installing a pyopencl with a lower cl version, e.g. cl12 : pyopencl=2020.1. However, in this case,
-you will need an environment with a lower python version (python=3.8).
-
 - `Error: Could not build wheels for hdbscan which use PEP 517 and cannot be installed directly`
 
 This can happen if you used pip for the installation. To solve this error, install hdbscan via conda before installing the plugin:
 
 ```
-conda install -c conda-forge hdbscan
+mamba install -c conda-forge hdbscan
 ```
 
 - `ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 96 from C header, got 88 from PyObject`
 
 Similar to the above-described error, this error can occur when importing hdbscan through pip or in the wrong order. This can be fixed by installing packages separately through conda and in the following order:
 ```bash
-conda install -c conda-forge napari pyopencl hdbscan
+mamba install -c conda-forge napari hdbscan
 pip install napari-clusters-plotter
 ```
 
-- `WARNING: No ICDs were found` or `LogicError: clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR`
-
-Make your system-wide implementation visible by installing either of the following conda packages:
-
-```
-conda install -c conda-forge ocl-icd-system
-conda install -c conda-forge ocl_icd_wrapper_apple
-```
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [pytest], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_Qt_code.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_Qt_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
+import typing
 from pathlib import Path as PathL
 
 import numpy as np
+import numpy.typing
+import pandas as pd
 from magicgui.widgets import create_widget
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
 from matplotlib.path import Path
-from matplotlib.widgets import LassoSelector, RectangleSelector
+from matplotlib.widgets import LassoSelector, RectangleSelector, SpanSelector
 from napari.layers import Image, Labels
 from qtpy.QtCore import QRect
 from qtpy.QtGui import QIcon
 from qtpy.QtWidgets import (
     QAbstractItemView,
     QHBoxLayout,
     QLabel,
@@ -347,14 +350,111 @@
         value=value,
         options=options,
     )
     container.layout().addWidget(choice_list.native)
     return container, choice_list
 
 
+def create_options_dropdown(name: str, value, options: dict, label: str):
+    """
+    Create a widget for selecting a value from a set of options.
+
+    Parameters
+    ----------
+    name : str
+        The name to be used for the widget.
+    value :
+        The initial value of the widget.
+    options : dict
+        A dictionary of possible options, where the keys are option
+        names and the values are corresponding strings that are
+        actually displayed in the combobox.
+    label : str
+        The label to be displayed next to the widget.
+
+    Returns
+    ----------
+    A tuple containing the container widget and the choice widget. The container widget
+    is a QWidget that contains the label and the choice widget.
+    """
+    container = QWidget()
+    container.setLayout(QHBoxLayout())
+    container.layout().addWidget(QLabel(label))
+    choice_list = create_widget(
+        widget_type="ComboBox",
+        name=name,
+        value=value,
+        options=options,
+    )
+    container.layout().addWidget(choice_list.native)
+    return container, choice_list
+
+
+class SelectFrom2DHistogram:
+    def __init__(self, parent, ax, full_data):
+        self.parent = parent
+        self.ax = ax
+        self.canvas = ax.figure.canvas
+        self.xys = full_data
+
+        self.lasso = LassoSelector(ax, onselect=self.onselect)
+        self.ind = []
+        self.ind_mask = []
+
+    def onselect(self, verts):
+        path = Path(verts)
+
+        self.ind_mask = path.contains_points(self.xys)
+        self.ind = np.nonzero(self.ind_mask)[0]
+
+        if self.parent.manual_clustering_method is not None:
+            self.parent.manual_clustering_method(self.ind_mask)
+
+    def disconnect(self):
+        self.lasso.disconnect_events()
+        self.canvas.draw_idle()
+
+
+class SelectFrom1DHistogram:
+    def __init__(self, parent, ax, full_data):
+        self.parent = parent
+        self.ax = ax
+        self.canvas = ax.figure.canvas
+        self.xys = full_data
+
+        self.span_selector = SpanSelector(
+            ax,
+            onselect=self.onselect,
+            direction="horizontal",
+            props=dict(facecolor="#1f77b4", alpha=0.5),
+        )
+        self.click_id = self.canvas.mpl_connect("button_press_event", self.on_click)
+
+    def onselect(self, vmin, vmax):
+        self.ind_mask = np.logical_and(self.xys >= vmin, self.xys <= vmax).values
+
+        if self.parent.manual_clustering_method is not None:
+            self.parent.manual_clustering_method(self.ind_mask)
+
+    def on_click(self, event):
+        # Clear selection if user right-clicks (without moving) outside of the histogram
+        if event.inaxes != self.ax:
+            return
+        if event.button == 3:
+            # clear selection
+            self.ind_mask = np.zeros_like(self.xys, dtype=bool)
+            if self.parent.manual_clustering_method is not None:
+                self.parent.manual_clustering_method(self.ind_mask)
+
+    def disconnect(self):
+        self.span_selector.disconnect_events()
+        self.canvas.mpl_disconnect(self.click_id)
+        self.canvas.draw_idle()
+
+
 # Class below was based upon matplotlib lasso selection example:
 # https://matplotlib.org/stable/gallery/widgets/lasso_selector_demo_sgskip.html
 class SelectFromCollection:
     """
     Select indices from a matplotlib collection using `LassoSelector`.
 
     Selected indices are saved in the `ind` attribute. This tool fades out the
@@ -394,16 +494,17 @@
 
         self.lasso = LassoSelector(ax, onselect=self.onselect, button=1)
         self.ind = []
         self.ind_mask = []
 
     def onselect(self, verts):
         path = Path(verts)
-        self.ind = np.nonzero(path.contains_points(self.xys))[0]
         self.ind_mask = path.contains_points(self.xys)
+        self.ind = np.nonzero(self.ind_mask)[0]
+
         self.fc[:, -1] = self.alpha_other
         self.fc[self.ind, -1] = 1
         self.collection.set_facecolors(self.fc)
         self.canvas.draw_idle()
         self.selected_coordinates = self.xys[self.ind].data
 
         if self.parent.manual_clustering_method is not None:
@@ -418,34 +519,47 @@
 
 class MplCanvas(FigureCanvas):
     def __init__(self, parent=None, width=7, height=4, manual_clustering_method=None):
         self.fig = Figure(figsize=(width, height), constrained_layout=True)
         self.manual_clustering_method = manual_clustering_method
 
         self.axes = self.fig.add_subplot(111)
+        self.histogram = None
 
         self.match_napari_layout()
+        self.xylim = None
 
         super().__init__(self.fig)
+        self.mpl_connect("draw_event", self.on_draw)
 
         self.pts = self.axes.scatter([], [])
         self.selector = SelectFromCollection(self, self.axes, self.pts)
         self.rectangle_selector = RectangleSelector(
             self.axes,
             self.draw_rectangle,
             useblit=True,
             props=dict(edgecolor="white", fill=False),
             button=3,  # right button
             minspanx=5,
             minspany=5,
             spancoords="pixels",
             interactive=False,
         )
+        self.selected_colormap = "magma"
+
         self.reset()
 
+    def reset_zoom(self):
+        if self.xylim:
+            self.axes.set_xlim(self.xylim[0])
+            self.axes.set_ylim(self.xylim[1])
+
+    def on_draw(self, event):
+        self.xylim = (self.axes.get_xlim(), self.axes.get_ylim())
+
     def draw_rectangle(self, eclick, erelease):
         """eclick and erelease are the press and release events"""
         x0, y0 = eclick.xdata, eclick.ydata
         x1, y1 = erelease.xdata, erelease.ydata
         self.xys = self.pts.get_offsets()
         min_x = min(x0, x1)
         max_x = max(x0, x1)
@@ -458,14 +572,97 @@
         if self.manual_clustering_method is not None:
             self.manual_clustering_method(self.rect_ind_mask)
 
     def reset(self):
         self.axes.clear()
         self.is_pressed = None
 
+    def make_2d_histogram(
+        self,
+        data_x: "numpy.typing.ArrayLike",
+        data_y: "numpy.typing.ArrayLike",
+        colors: "typing.List[str]",
+        bin_number: int = 400,
+        log_scale: bool = False,
+    ):
+        self.colors = colors
+        norm = None
+        if log_scale:
+            norm = "log"
+        h, xedges, yedges = np.histogram2d(data_x, data_y, bins=bin_number)
+        self.axes.imshow(
+            h.T,
+            extent=[xedges[0], xedges[-1], yedges[0], yedges[-1]],
+            origin="lower",
+            cmap=self.selected_colormap,
+            aspect="auto",
+            norm=norm,
+        )
+        self.axes.set_xlim(xedges[0], xedges[-1])
+        self.axes.set_ylim(yedges[0], yedges[-1])
+        self.histogram = (h, xedges, yedges)
+
+        full_data = pd.concat([pd.DataFrame(data_x), pd.DataFrame(data_y)], axis=1)
+        self.selector.disconnect()
+        self.selector = SelectFrom2DHistogram(self, self.axes, full_data)
+        self.axes.figure.canvas.draw_idle()
+
+    def make_1d_histogram(
+        self,
+        data: "numpy.typing.ArrayLike",
+        bin_number: int = 400,
+        log_scale: bool = False,
+    ):
+        counts, bins = np.histogram(data, bins=bin_number)
+        self.axes.hist(
+            bins[:-1],
+            bins,
+            edgecolor="white",
+            weights=counts,
+            log=log_scale,
+            color="#9A9A9A",
+        )
+        self.histogram = (counts, bins)
+        bin_width = bins[1] - bins[0]
+        self.axes.set_xlim(min(bins) - (bin_width / 2), max(bins) + (bin_width / 2))
+        ymin = 0
+        if log_scale:
+            ymin = 1
+        self.axes.set_ylim(ymin, max(counts) * 1.1)
+
+        if log_scale:
+            self.axes.set_xscale("linear")
+            self.axes.set_yscale("log")
+
+        self.selector.disconnect()
+        self.selector = SelectFrom1DHistogram(self, self.axes, data)
+        self.axes.figure.canvas.draw_idle()
+
+    def make_scatter_plot(
+        self,
+        data_x: "numpy.typing.ArrayLike",
+        data_y: "numpy.typing.ArrayLike",
+        colors: "typing.List[str]",
+        sizes: "typing.List[float]",
+        alpha: "typing.List[float]",
+    ):
+        self.pts = self.axes.scatter(
+            data_x,
+            data_y,
+            c=colors,
+            s=sizes,
+            alpha=alpha,
+        )
+        self.selector.disconnect()
+        self.selector = SelectFromCollection(
+            self,
+            self.axes,
+            self.pts,
+        )
+
     def match_napari_layout(self):
         """Change background and axes colors to match napari layout"""
         # changing color of axes background to napari main window color
         self.fig.patch.set_facecolor("#262930")
         # changing color of plot background to napari main window color
         self.axes.set_facecolor("#262930")
 
@@ -480,14 +677,15 @@
         # changing colors of axes ticks
         self.axes.tick_params(axis="x", colors="white", labelcolor="white")
         self.axes.tick_params(axis="y", colors="white", labelcolor="white")
 
         # changing colors of axes labels
         self.axes.xaxis.label.set_color("white")
         self.axes.yaxis.label.set_color("white")
+        self.fig.canvas.draw_idle()
 
 
 # overriding NavigationToolbar method to change the background and axes colors of saved figure
 class MyNavigationToolbar(NavigationToolbar):
     def __init__(self, canvas, parent):
         super().__init__(canvas, parent)
         self.canvas = canvas
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_clustering.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import numpy as np
 import pandas as pd
 from napari.qt.threading import create_worker
 from napari_tools_menu import register_dock_widget
 from qtpy.QtWidgets import QHBoxLayout, QLabel, QLineEdit, QVBoxLayout, QWidget
 
 from ._Qt_code import (
-    algorithm_choice,
     button,
     checkbox,
+    create_options_dropdown,
     float_sbox_containter_and_selection,
     int_sbox_containter_and_selection,
     labels_container_and_selection,
     measurements_container_and_list,
     title,
 )
 from ._utilities import (
@@ -73,15 +73,18 @@
         # widget for the selection of properties to perform clustering
         (
             choose_properties_container,
             self.properties_list,
         ) = measurements_container_and_list()
 
         # selection of the clustering methods
-        self.clust_method_container, self.clust_method_choice_list = algorithm_choice(
+        (
+            self.clust_method_container,
+            self.clust_method_choice_list,
+        ) = create_options_dropdown(
             name="Clustering_method",
             value=self.Options.EMPTY.value,
             options={"choices": [e.value for e in self.Options]},
             label="Clustering Method",
         )
 
         # clustering options for KMeans
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_dimensionality_reduction.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dimensionality_reduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from functools import partial
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from napari.qt.threading import create_worker
 from napari_tools_menu import register_dock_widget
-from qtpy.QtWidgets import QVBoxLayout, QWidget
+from qtpy.QtWidgets import QHBoxLayout, QLabel, QLineEdit, QVBoxLayout, QWidget
 
 from ._clustering import ID_NAME
 from ._plotter import POINTER
 from ._Qt_code import (
-    algorithm_choice,
     button,
     checkbox,
     collapsible_box,
+    create_options_dropdown,
     float_sbox_containter_and_selection,
     int_sbox_containter_and_selection,
     labels_container_and_selection,
     measurements_container_and_list,
     title,
 )
 from ._utilities import (
@@ -34,27 +34,32 @@
     widgets_active,
     widgets_valid,
 )
 
 # Remove when the problem is fixed from sklearn side
 warnings.filterwarnings(action="ignore", category=FutureWarning, module="sklearn")
 
-DEBUG = False
 
 DEFAULTS = {
     "n_neighbors": 15,
     "perplexity": 30,
     "standardization": True,
     "pca_components": 0,
     "explained_variance": 95.0,
     "n_components": 2,
     # enabling multithreading for UMAP can result in crashing kernel if napari is opened from the Jupyter notebook,
     # therefore by default the following value is False.
     # See more: https://github.com/BiAPoL/napari-clusters-plotter/issues/169
     "umap_separate_thread": False,
+    "min_distance_umap": 0.1,
+    "mds_n_init": 4,
+    "mds_metric": True,
+    "mds_max_iter": 300,
+    "mds_eps": 0.001,
+    "custom_name": "",
 }
 
 EXCLUDE = [ID_NAME, POINTER, "UMAP", "t-SNE", "PCA"]
 
 
 @register_dock_widget(
     menu="Measurement post-processing > Dimensionality reduction (ncp)"
@@ -87,15 +92,15 @@
         # select properties of which to produce a dimensionality reduced version
         (
             choose_properties_container,
             self.properties_list,
         ) = measurements_container_and_list()
 
         # selection of dimension reduction algorithm
-        algorithm_container, self.algorithm_choice_list = algorithm_choice(
+        algorithm_container, self.algorithm_choice_list = create_options_dropdown(
             name="Dimensionality_reduction_method",
             value=self.Options.EMPTY.value,
             options={"choices": [e.value for e in self.Options]},
             label="Dimensionality Reduction Method",
         )
 
         # selection of n_neighbors - The size of local neighborhood (in terms of number of neighboring sample points)
@@ -192,75 +197,100 @@
 
         # advanced options for UMAP
         self.advanced_options_container = collapsible_box("Expand for advanced options")
         self.advanced_options_container.setVisible(
             False
         )  # hide this container until umap is selected
 
-        self.settings_container_multithreading, self.multithreading = checkbox(
+        self.settings_container_multithreading, self.umap_separate_thread = checkbox(
             name="Enable Multi-threading",
             value=DEFAULTS["umap_separate_thread"],
             visible=True,
             tool_tip="Only enable if you are running napari not from the Jupyter notebook or your data is not big.\n"
             "Otherwise it can result in the crash of the kernel.",
         )
         self.advanced_options_container.addWidget(
             self.settings_container_multithreading
         )
 
+        (
+            self.min_distance_umap_container,
+            self.min_distance_umap,
+        ) = float_sbox_containter_and_selection(
+            name="Minimum Distance",
+            label="Minimum Distance",
+            value=DEFAULTS["min_distance_umap"],
+            step=0.1,
+            min=0,
+            visible=False,
+            tool_tip="The minimum distance apart that points are allowed to be in the low dimensional representation.",
+            tool_link="https://umap-learn.readthedocs.io/en/latest/parameters.html#min-dist",
+        )
+
         # additional options for MDS
         (self.mds_metric_container, self.mds_metric) = checkbox(
             "Metric",
-            value=True,
+            value=DEFAULTS["mds_metric"],
             visible=False,
             tool_tip="If selected perform metric MDS; otherwise, nonmetric MDS, where dissimilarities with 0 "
             "are considered as missing values.",
             tool_link="https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling",
         )
 
         (
             self.mds_n_init_container,
             self.mds_n_init,
         ) = int_sbox_containter_and_selection(
             name="Number of Initializations",
             label="Number of Initializations",
-            value=4,
+            value=DEFAULTS["mds_n_init"],
             min=1,
             visible=False,
             tool_tip="Number of times the SMACOF algorithm will be run with different"
             " initializations. The final results\nwill be the best output of"
             " the runs, determined by the run with the smallest final stress.",
             tool_link="https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling",
         )
 
         (
             self.mds_max_iter_container,
             self.mds_max_iter,
         ) = int_sbox_containter_and_selection(
             name="Max Number of Iterations",
             label="Max Number of Iterations",
-            value=300,
+            value=DEFAULTS["mds_max_iter"],
             min=1,
             visible=False,
             tool_tip="Maximum number of iterations of the SMACOF algorithm for a "
             "single run.",
             tool_link="https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling",
         )
 
         (self.mds_eps_container, self.mds_eps) = float_sbox_containter_and_selection(
             name="Relative Tolerance",
             label="Relative Tolerance",
-            value=0.001,
+            value=DEFAULTS["mds_eps"],
             min=0.00000001,
             visible=False,
             tool_tip="Relative tolerance with respect to stress at which to "
             "declare convergence.",
             tool_link="https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling",
         )
 
+        # custom result column name field
+        self.custom_name_container = QWidget()
+        self.custom_name_container.setLayout(QHBoxLayout())
+        self.custom_name_container.layout().addWidget(
+            QLabel("Optional Custom Results Name")
+        )
+        self.custom_name = QLineEdit()
+
+        self.custom_name_container.layout().addWidget(self.custom_name)
+        self.custom_name.setPlaceholderText("Algorithm_name")
+
         # making buttons
         run_container, self.run_button = button("Run")
         update_container, self.update_button = button("Update Measurements")
         defaults_container, self.defaults_button = button("Restore Defaults")
 
         def run_clicked():
             if self.labels_select.value is None:
@@ -282,19 +312,21 @@
                 self.n_neighbors.value,
                 self.perplexity.value,
                 self.algorithm_choice_list.current_choice,
                 self.standardization.value,
                 self.explained_variance.value,
                 self.pca_components.value,
                 self.n_components.value,
-                self.multithreading.value,
+                self.umap_separate_thread.value,
+                self.min_distance_umap.value,
                 self.mds_metric.value,
                 self.mds_n_init.value,
                 self.mds_max_iter.value,
                 self.mds_eps.value,
+                self.custom_name.text(),
             )
 
         # connect buttons with functions that need to be triggered by them
         self.run_button.clicked.connect(run_clicked)
         self.update_button.clicked.connect(
             partial(update_properties_list, self, EXCLUDE)
         )
@@ -314,22 +346,24 @@
         self.layout().addWidget(label_container)
         self.layout().addWidget(labels_layer_selection_container)
         self.layout().addWidget(algorithm_container)
         self.layout().addWidget(self.perplexity_container)
         self.layout().addWidget(self.n_neighbors_container)
         self.layout().addWidget(self.pca_components_container)
         self.layout().addWidget(self.n_components_container)
+        self.layout().addWidget(self.min_distance_umap_container)
         self.layout().addWidget(self.explained_variance_container)
         self.layout().addWidget(self.settings_container_scaler)
         self.layout().addWidget(self.mds_metric_container)
         self.layout().addWidget(self.mds_n_init_container)
         self.layout().addWidget(self.mds_max_iter_container)
         self.layout().addWidget(self.mds_eps_container)
         self.layout().addWidget(choose_properties_container)
         self.layout().addWidget(self.advanced_options_container)
+        self.layout().addWidget(self.custom_name_container)
         self.layout().addWidget(update_container)
         self.layout().addWidget(defaults_container)
         self.layout().addWidget(run_container)
         self.layout().setSpacing(0)
 
         # go through all widgets and change spacing
         for i in range(self.layout().count()):
@@ -352,30 +386,35 @@
     def _check_perplexity(self):
         """
         The function, which is triggered by the selection of t-SNE as a dimensionality reduction algorithm,
         change of input image or perplexity value. It checks whether the selected perplexity is less than
         the number of labeled objects, and if not it makes the widget red.
         """
         if self.algorithm_choice_list.current_choice == "t-SNE":
-            features = get_layer_tabular_data(self.labels_select.value)
-            widgets_valid(
-                self.perplexity, valid=self.perplexity.value <= features.shape[0]
-            )
-            if self.perplexity.value >= features.shape[0]:
-                warnings.warn(
-                    "Perplexity must be less than the number of labeled objects!"
+            if (
+                self.labels_select.value is not None
+                and get_layer_tabular_data(self.labels_select.value) is not None
+            ):
+                features = get_layer_tabular_data(self.labels_select.value)
+                widgets_valid(
+                    self.perplexity, valid=self.perplexity.value <= features.shape[0]
                 )
+                if self.perplexity.value >= features.shape[0]:
+                    warnings.warn(
+                        "Perplexity must be less than the number of labeled objects!"
+                    )
 
     def change_settings_visibility(self):
         """
         The function, which is triggered by the selection/change of dimensionality reduction algorithm.
         It changes the visibility of some parameters depending on the current choice of the algorithm.
         """
         widgets_active(
             self.n_neighbors_container,
+            self.min_distance_umap_container,
             self.advanced_options_container,
             active=self.algorithm_choice_list.current_choice == self.Options.UMAP.value,
         )
         widgets_active(
             self.n_neighbors_container,
             active=self.algorithm_choice_list.current_choice
             == self.Options.ISOMAP.value,
@@ -430,39 +469,34 @@
         perplexity,
         selected_algorithm,
         standardize,
         explained_variance,
         pca_components,
         n_components,
         umap_multithreading,
+        min_dist,
         mds_metric,
         mds_n_init,
         mds_max_iter,
         mds_eps,
+        custom_name,
     ):
         """
         The function triggered by clicking the run button.
         """
         print("Selected labels layer: " + str(labels_layer))
         print("Selected measurements: " + str(selected_measurements_list))
 
         def activate_buttons(error=None, active=True):
             """Utility function to enable all the buttons again if an error/exception happens in a secondary thread or
             the computation has finished successfully."""
 
             buttons_active(
                 self.run_button, self.defaults_button, self.update_button, active=active
             )
-            if DEBUG:
-                print(error)
-                print("Buttons are activated again")
-
-            if DEBUG:
-                print(error)
-                print("Buttons are activated again")
 
         # disable all the buttons while the computation is happening
         activate_buttons(active=False)
 
         # try statement is added to catch any exceptions/errors and enable all the buttons again if that is the case
         try:
             features = get_layer_tabular_data(labels_layer)
@@ -503,31 +537,45 @@
                         if column.startswith("PC_")
                     ]
                     df_principal_components_removed = tabular_data.drop(
                         dropkeys, axis=1
                     )
                     set_features(labels_layer, df_principal_components_removed)
 
+                    result_column_name = (
+                        "PC_" if custom_name == DEFAULTS["custom_name"] else custom_name
+                    )
+
                     # write result back to properties/features of the layer
                     for i in range(0, len(result[1].T)):
                         add_column_to_layer_tabular_data(
-                            labels_layer, "PC_" + str(i), result[1][:, i]
+                            labels_layer,
+                            str(result_column_name) + str(i),
+                            result[1][:, i],
                         )
 
                 elif (
                     result[0] == "UMAP"
                     or result[0] == "t-SNE"
                     or result[0] == "Isomap"
                     or result[0] == "MDS"
                 ):
                     # write result back to properties/features of the layer
-                    for i in range(0, n_components):
-                        add_column_to_layer_tabular_data(
-                            labels_layer, result[0] + "_" + str(i), result[1][:, i]
-                        )
+                    if custom_name == DEFAULTS["custom_name"]:
+                        for i in range(0, n_components):
+                            add_column_to_layer_tabular_data(
+                                labels_layer, result[0] + "_" + str(i), result[1][:, i]
+                            )
+                    else:
+                        for i in range(0, n_components):
+                            add_column_to_layer_tabular_data(
+                                labels_layer,
+                                custom_name + "_" + str(i),
+                                result[1][:, i],
+                            )
 
                 else:
                     "Dimensionality reduction not successful. Please try again"
                     return
 
                 # add a table to napari viewer
                 show_table(viewer, labels_layer)
@@ -540,14 +588,15 @@
             ):
                 # this part runs if umap is selected, and the multithreading is enabled under advanced options
                 self.worker = create_worker(
                     umap,
                     properties_to_reduce,
                     n_neighbors=n_neighbours,
                     n_components=n_components,
+                    min_dist=min_dist,
                     verbose=True,
                     _progress=True,
                 )
                 self.worker.returned.connect(return_func_dim_reduction)
                 self.worker.errored.connect(activate_buttons)
                 self.worker.start()
 
@@ -558,14 +607,15 @@
                 # this part runs if umap is selected, and the progress bar/multithreading is disabled (default option)
                 # enabling multithreading for UMAP can result in crashing kernel if napari is opened from the notebook
                 # See more: https://github.com/BiAPoL/napari-clusters-plotter/issues/169
                 result = umap(
                     properties_to_reduce,
                     n_neighbors=n_neighbours,
                     n_components=n_components,
+                    min_dist=min_dist,
                     verbose=False,
                 )
 
                 return_func_dim_reduction(result)
 
             elif selected_algorithm == self.Options.TSNE.value:
                 self.worker = create_worker(
@@ -622,15 +672,19 @@
             # make buttons active again even if an exception occurred during execution
             # of the code above and not in a secondary thread
             activate_buttons()
 
 
 @catch_NaNs
 def umap(
-    reg_props: pd.DataFrame, n_neighbors: int, n_components: int, verbose: bool = False
+    reg_props: pd.DataFrame,
+    n_neighbors: int,
+    n_components: int,
+    min_dist: float,
+    verbose: bool = False,
 ) -> Tuple[str, np.ndarray]:
     """
     Performs dimensionality reduction using the Uniform Manifold Approximation Projection (UMAP) on the given data.
     UMAP is a nonlinear dimensionality reduction technique that preserves the global structure of the data while
     allowing for efficient computation of distances in the lower-dimensional space.
 
     Parameters
@@ -660,14 +714,15 @@
     import umap.umap_ as umap
 
     reducer = umap.UMAP(
         random_state=133,
         n_components=n_components,
         n_neighbors=n_neighbors,
         verbose=verbose,
+        min_dist=min_dist,
         tqdm_kwds={"desc": "Dimensionality reduction progress"},
     )
     return "UMAP", reducer.fit_transform(reg_props)
 
 
 @catch_NaNs
 def tsne(
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_plotter.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,92 @@
 import os
 import warnings
+from enum import Enum, auto
 
 import numpy as np
 import pandas as pd
+from matplotlib.figure import Figure
+from napari.utils.colormaps import ALL_COLORMAPS
 from napari_tools_menu import register_dock_widget
 from qtpy import QtWidgets
 from qtpy.QtCore import Qt
 from qtpy.QtGui import QGuiApplication, QIcon
 from qtpy.QtWidgets import (
     QCheckBox,
     QComboBox,
     QHBoxLayout,
     QLabel,
     QMainWindow,
+    QPushButton,
     QScrollArea,
+    QSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
-from ._plotter_utilities import clustered_plot_parameters, unclustered_plot_parameters
+from ._plotter_utilities import (
+    apply_cluster_colors_to_bars,
+    clustered_plot_parameters,
+    estimate_number_bins,
+    make_cluster_overlay_img,
+    unclustered_plot_parameters,
+)
 from ._Qt_code import (
     ICON_ROOT,
     MplCanvas,
     MyNavigationToolbar,
-    SelectFromCollection,
     button,
     collapsible_box,
+    create_options_dropdown,
     labels_container_and_selection,
     title,
 )
 from ._utilities import (
     add_column_to_layer_tabular_data,
     dask_cluster_image_timelapse,
     generate_cluster_image,
     get_layer_tabular_data,
     get_nice_colormap,
 )
 
 POINTER = "frame"
 
+POSSIBLE_CLUSTER_IDS = ["KMEANS", "HDBSCAN", "MS", "GMM", "AC"]  # not including manual
+
+
+class PlottingType(Enum):
+    HISTOGRAM = auto()
+    SCATTER = auto()
+
 
 @register_dock_widget(menu="Measurement > Plot measurements (ncp)")
 @register_dock_widget(menu="Visualization > Plot measurements (ncp)")
 class PlotterWidget(QMainWindow):
     def __init__(self, napari_viewer):
         super().__init__()
 
         self.cluster_ids = None
         self.viewer = napari_viewer
 
         # create a scroll area
         self.scrollArea = QScrollArea()
         self.setCentralWidget(self.scrollArea)
         self.scrollArea.setWidgetResizable(True)
-        self.scrollArea.setMinimumWidth(400)
+        self.scrollArea.setMinimumWidth(450)
         self.scrollArea.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
 
         self.contents = QWidget()
         self.scrollArea.setWidget(self.contents)
 
         self.layout = QVBoxLayout(self.contents)
         self.layout.setAlignment(Qt.AlignTop)
 
+        # a figure instance to plot on
+        self.figure = Figure()
+
         self.analysed_layer = None
         self.visualized_labels_layer = None
 
         def manual_clustering_method(inside):
             inside = np.array(inside)  # leads to errors sometimes otherwise
 
             if self.analysed_layer is None or len(inside) == 0:
@@ -81,27 +102,31 @@
                 features.update(pd.DataFrame(former_clusters, columns=[clustering_ID]))
             else:
                 features[clustering_ID] = inside.astype(int)
             add_column_to_layer_tabular_data(
                 self.analysed_layer, clustering_ID, features[clustering_ID]
             )
 
+            # update the dropdown, so that the "MANUAL_CLUSTER_ID" is added
+            self.update_axes_and_clustering_id_lists()
+            # set the selected item of the "clustering" combobox
+            self.plot_cluster_id.setCurrentText(clustering_ID)
+
             # redraw the whole plot
             self.run(
                 features,
                 self.plot_x_axis_name,
                 self.plot_y_axis_name,
                 plot_cluster_name=clustering_ID,
             )
-            self.labels_select.value.visible = False
+            self.labels_select.value.opacity = 0
 
-        # Canvas Widget that displays the 'figure'
-        # fig instance is created inside MplCanvas
+        # Canvas Widget that displays the 'figure', it takes the 'figure' instance
         self.graphics_widget = MplCanvas(
-            manual_clustering_method=manual_clustering_method
+            self.figure, manual_clustering_method=manual_clustering_method
         )
 
         # Navigation widget
         self.toolbar = MyNavigationToolbar(self.graphics_widget, self)
 
         # Modify toolbar icons and some tooltips
         for action in self.toolbar.actions():
@@ -148,56 +173,172 @@
         cluster_container = QWidget()
         cluster_container.setLayout(QHBoxLayout())
         cluster_container.layout().addWidget(QLabel("Clustering"))
         self.plot_cluster_id = QComboBox()
         cluster_container.layout().addWidget(self.plot_cluster_id)
 
         # making buttons
-        run_container, run_button = button("Run")
-        update_container, update_button = button("Update Measurements")
+        run_container, run_button = button("Plot")
+        update_container, update_button = button("Update Axes/Clustering Options")
 
-        # checkbox background
-        self.advanced_options_container = collapsible_box("Expand for advanced options")
+        ############################
+        # Advanced plotting options
+        ############################
 
-        def checkbox_status_changed():
+        self.advanced_options_container_box = collapsible_box(
+            "Expand for advanced options"
+        )
+        self.advanced_options_container = QWidget(self)
+        self.advanced_options_container.setLayout(QVBoxLayout())
+        self.advanced_options_container_box.addWidget(self.advanced_options_container)
+        self.advanced_options_container.layout().setSpacing(0)
+        self.advanced_options_container.layout().setContentsMargins(0, 0, 0, 0)
+
+        def replot():
+            clustering_ID = None
             if self.cluster_ids is not None:
-                clustering_ID = "MANUAL_CLUSTER_ID"
-                features = get_layer_tabular_data(self.analysed_layer)
+                clustering_ID = self.plot_cluster_id.currentText()
+
+            features = get_layer_tabular_data(self.analysed_layer)
 
-                # redraw the whole plot
+            # redraw the whole plot
+            try:
                 self.run(
                     features,
                     self.plot_x_axis_name,
                     self.plot_y_axis_name,
                     plot_cluster_name=clustering_ID,
                 )
 
-        checkbox_container = QWidget()
-        checkbox_container.setLayout(QHBoxLayout())
-        checkbox_container.layout().addWidget(QLabel("Hide non-selected clusters"))
+            except AttributeError:
+                # In this case, replotting is not yet possible
+                pass
+
+        def checkbox_status_changed():
+            replot()
+
+        def plotting_type_changed():
+            if self.plotting_type.currentText() == PlottingType.HISTOGRAM.name:
+                self.bin_number_container.setVisible(True)
+                self.log_scale_container.setVisible(True)
+                self.plot_hide_non_selected.setChecked(True)
+                self.colormap_container.setVisible(True)
+            else:
+                self.bin_number_container.setVisible(False)
+                self.log_scale_container.setVisible(False)
+                self.colormap_container.setVisible(False)
+            replot()
+
+        def bin_number_set():
+            replot()
+
+        def bin_auto():
+            self.bin_number_manual_container.setVisible(not self.bin_auto.isChecked())
+            if self.bin_auto.isChecked():
+                replot()
+
+        # Combobox with plotting types
+        combobox_plotting_container = QWidget()
+        combobox_plotting_container.setLayout(QHBoxLayout())
+        combobox_plotting_container.layout().addWidget(QLabel("Plotting type"))
+        self.plotting_type = QComboBox()
+        self.plotting_type.addItems(
+            [PlottingType.SCATTER.name, PlottingType.HISTOGRAM.name]
+        )
+        self.plotting_type.currentIndexChanged.connect(plotting_type_changed)
+        combobox_plotting_container.layout().addWidget(self.plotting_type)
+
+        self.bin_number_container = QWidget()
+        self.bin_number_container.setLayout(QHBoxLayout())
+        self.bin_number_container.layout().addWidget(QLabel("Number of bins"))
+
+        self.bin_number_manual_container = QWidget()
+        self.bin_number_manual_container.setLayout(QHBoxLayout())
+        self.bin_number_spinner = QSpinBox()
+        self.bin_number_spinner.setMinimum(1)
+        self.bin_number_spinner.setMaximum(1000)
+        self.bin_number_spinner.setValue(400)
+
+        self.bin_number_manual_container.layout().addWidget(self.bin_number_spinner)
+        self.bin_number_set = QPushButton("Set")
+        self.bin_number_set.clicked.connect(bin_number_set)
+        self.bin_number_manual_container.layout().addWidget(self.bin_number_set)
+
+        self.bin_number_container.layout().addWidget(self.bin_number_manual_container)
+
+        self.bin_auto = QCheckBox("Auto")
+        self.bin_auto.setChecked(True)
+        self.bin_auto.stateChanged.connect(bin_auto)
+        self.bin_number_container.layout().addWidget(self.bin_auto)
+
+        self.bin_number_manual_container.setVisible(False)
+        self.bin_number_container.setVisible(False)
+
+        self.log_scale_container = QWidget()
+        self.log_scale_container.setLayout(QHBoxLayout())
+        self.log_scale_container.layout().addWidget(QLabel("Log scale"))
+        self.log_scale = QCheckBox("")
+        self.log_scale.setChecked(False)
+        self.log_scale.stateChanged.connect(replot)
+        self.log_scale_container.layout().addWidget(self.log_scale)
+
+        self.log_scale_container.setVisible(False)
+
+        # Checkbox to hide non-selected clusters
+        self.hide_nonselected_checkbox_container = QWidget()
+        self.hide_nonselected_checkbox_container.setLayout(QHBoxLayout())
+        self.hide_nonselected_checkbox_container.layout().addWidget(
+            QLabel("Hide non-selected clusters")
+        )
         self.plot_hide_non_selected = QCheckBox()
+        self.plot_hide_non_selected.setToolTip("Enabled only for manual clustering")
         self.plot_hide_non_selected.stateChanged.connect(checkbox_status_changed)
-        checkbox_container.layout().addWidget(self.plot_hide_non_selected)
-        self.advanced_options_container.addWidget(checkbox_container)
+        self.hide_nonselected_checkbox_container.layout().addWidget(
+            self.plot_hide_non_selected
+        )
+
+        self.advanced_options_container.layout().addWidget(combobox_plotting_container)
+        self.advanced_options_container.layout().addWidget(self.log_scale_container)
+        self.advanced_options_container.layout().addWidget(self.bin_number_container)
+        self.advanced_options_container.layout().addWidget(
+            self.hide_nonselected_checkbox_container
+        )
+
+        # selection of possible colormaps for 2D histogram
+        self.colormap_container, self.colormap_dropdown = create_options_dropdown(
+            name="Colormap",
+            value="magma",
+            options={"choices": list(ALL_COLORMAPS.keys())},
+            label="Colormap",
+        )
+        self.colormap_container.setVisible(False)
+        self.colormap_dropdown.native.currentIndexChanged.connect(replot)
+        self.advanced_options_container.layout().addWidget(self.colormap_container)
 
         # adding all widgets to the layout
         self.layout.addWidget(label_container, alignment=Qt.AlignTop)
         self.layout.addWidget(labels_layer_selection_container, alignment=Qt.AlignTop)
         self.layout.addWidget(axes_container, alignment=Qt.AlignTop)
         self.layout.addWidget(cluster_container, alignment=Qt.AlignTop)
-        self.layout.addWidget(self.advanced_options_container)
+
+        self.layout.addWidget(
+            self.advanced_options_container_box, alignment=Qt.AlignTop
+        )
+
         self.layout.addWidget(update_container, alignment=Qt.AlignTop)
         self.layout.addWidget(run_container, alignment=Qt.AlignTop)
         self.layout.setSpacing(0)
 
         # go through all widgets and change spacing
-        for i in range(self.layout.count()):
-            item = self.layout.itemAt(i).widget()
-            item.layout().setSpacing(0)
-            item.layout().setContentsMargins(3, 3, 3, 3)
+        for widget_list in [self.layout, self.advanced_options_container.layout()]:
+            for i in range(widget_list.count()):
+                item = widget_list.itemAt(i).widget()
+                if item.layout() is not None:
+                    item.layout().setSpacing(0)
+                    item.layout().setContentsMargins(3, 3, 3, 3)
 
         # adding spacing between fields for selecting two axes
         axes_container.layout().setSpacing(6)
 
         def run_clicked():
             if self.labels_select.value is None:
                 warnings.warn("Please select labels layer!")
@@ -224,83 +365,107 @@
                 self.plot_y_axis.currentText(),
                 self.plot_cluster_id.currentText(),
             )
 
         # takes care of case where this isn't set yet directly after init
         self.plot_cluster_name = None
         self.old_frame = None
+        # Assume time is the first axis
         self.frame = self.viewer.dims.current_step[0]
 
-        def frame_changed(event):
-            if self.viewer.dims.ndim <= 3:
-                return
-            frame = event.value[0]
-            if (not self.old_frame) or (self.old_frame != frame):
-                if self.labels_select.value is None:
-                    warnings.warn("Please select labels layer!")
-                    return
-                if get_layer_tabular_data(self.labels_select.value) is None:
-                    warnings.warn(
-                        "No labels image with features/properties was selected! Consider doing measurements first."
-                    )
-                    return
-                if (
-                    self.plot_x_axis.currentText() == ""
-                    or self.plot_y_axis.currentText() == ""
-                ):
-                    warnings.warn(
-                        "No axis(-es) was/were selected! If you cannot see anything in axes selection boxes, "
-                        "but you have performed measurements/dimensionality reduction before, try clicking "
-                        "Update Axes Selection Boxes"
-                    )
-                    return
-
-                self.frame = frame
-
-                self.run(
-                    get_layer_tabular_data(self.labels_select.value),
-                    self.plot_x_axis.currentText(),
-                    self.plot_y_axis.currentText(),
-                    self.plot_cluster_name,
-                    redraw_cluster_image=False,
-                )
-            self.old_frame = frame
-
         # update axes combo boxes once a new label layer is selected
-        self.labels_select.changed.connect(self.update_axes_list)
+        self.labels_select.changed.connect(self.update_axes_and_clustering_id_lists)
+        # depending on the select clustering ID, enable/disable the checkbox for hiding clusters
+        self.plot_cluster_id.currentIndexChanged.connect(
+            self.change_state_of_nonselected_checkbox
+        )
 
         # update axes combo boxes automatically if features of
         # layer are changed
         self.last_connected = None
         self.labels_select.changed.connect(self.activate_property_autoupdate)
 
         # update axes combo boxes once update button is clicked
-        update_button.clicked.connect(self.update_axes_list)
+        update_button.clicked.connect(self.update_axes_and_clustering_id_lists)
 
         # select what happens when the run button is clicked
         run_button.clicked.connect(run_clicked)
 
-        self.viewer.dims.events.current_step.connect(frame_changed)
+        self.viewer.dims.events.current_step.connect(self.frame_changed)
 
-        self.update_axes_list()
+        self.update_axes_and_clustering_id_lists()
+
+    def frame_changed(self, event):
+        if self.viewer.dims.ndim <= 3:
+            return
+        frame = event.value[0]
+        if (not self.old_frame) or (self.old_frame != frame):
+            if self.labels_select.value is None:
+                warnings.warn("Please select labels layer!")
+                return
+            if get_layer_tabular_data(self.labels_select.value) is None:
+                warnings.warn(
+                    "No labels image with features/properties was selected! Consider doing measurements first."
+                )
+                return
+            if (
+                self.plot_x_axis.currentText() == ""
+                or self.plot_y_axis.currentText() == ""
+            ):
+                warnings.warn(
+                    "No axis(-es) was/were selected! If you cannot see anything in axes selection boxes, "
+                    "but you have performed measurements/dimensionality reduction before, try clicking "
+                    "Update Axes Selection Boxes"
+                )
+                return
+
+            self.frame = frame
+
+            self.run(
+                get_layer_tabular_data(self.labels_select.value),
+                self.plot_x_axis.currentText(),
+                self.plot_y_axis.currentText(),
+                self.plot_cluster_name,
+                redraw_cluster_image=False,
+            )
+        self.old_frame = frame
 
     def showEvent(self, event) -> None:
         super().showEvent(event)
         self.reset_choices()
 
     def reset_choices(self, event=None):
         self.labels_select.reset_choices(event)
 
+    def change_state_of_nonselected_checkbox(self):
+        # make the checkbox visible only if clustering is done manually
+        visible = (
+            True
+            if "MANUAL_CLUSTER_ID" in self.plot_cluster_id.currentText()
+            or self.plot_cluster_id.currentText() == ""
+            else False
+        )
+        self.hide_nonselected_checkbox_container.setVisible(visible)
+
+        if any(
+            name in self.plot_cluster_id.currentText() for name in POSSIBLE_CLUSTER_IDS
+        ):
+            self.plot_hide_non_selected.setChecked(False)
+
     def activate_property_autoupdate(self):
         if self.last_connected is not None:
-            self.last_connected.events.properties.disconnect(self.update_axes_list)
-        self.labels_select.value.events.properties.connect(self.update_axes_list)
+            self.last_connected.events.properties.disconnect(
+                self.update_axes_and_clustering_id_lists
+            )
+        self.labels_select.value.events.properties.connect(
+            self.update_axes_and_clustering_id_lists
+        )
         self.last_connected = self.labels_select.value
 
-    def update_axes_list(self):
+    def update_axes_and_clustering_id_lists(self):
         selected_layer = self.labels_select.value
 
         former_x_axis = self.plot_x_axis.currentIndex()
         former_y_axis = self.plot_y_axis.currentIndex()
         former_cluster_id = self.plot_cluster_id.currentIndex()
 
         if selected_layer is not None:
@@ -331,14 +496,15 @@
         plot_cluster_name=None,
         redraw_cluster_image=True,
         force_redraw: bool = False,
     ):
         """
         This function that runs after the run button is clicked.
         """
+
         if not self.isVisible() and force_redraw is False:
             # don't redraw in case the plot is invisible anyway
             return
 
         # check whether given axes names exist and if not don't redraw
         if (
             plot_x_axis_name not in features.columns
@@ -353,74 +519,134 @@
         self.data_y = features[plot_y_axis_name]
         self.plot_x_axis_name = plot_x_axis_name
         self.plot_y_axis_name = plot_y_axis_name
         self.plot_cluster_name = plot_cluster_name
         self.analysed_layer = self.labels_select.value
 
         self.graphics_widget.reset()
+
+        self.graphics_widget.selected_colormap = self.colormap_dropdown.value
+
         number_of_points = len(features)
 
         # if selected image is 4 dimensional, but does not contain frame column in its features
         # it will be considered to be tracking data, where all labels of the same track have
         # the same label, and each column represent track's features
-        tracking_data = (
-            len(self.analysed_layer.data.shape) == 4 and "frame" not in features.keys()
-        )
-
+        tracking_data = len(self.analysed_layer.data.shape) == 4 and "frame" not in [
+            key.lower() for key in features.keys()
+        ]
+        colors = get_nice_colormap()
         if (
             plot_cluster_name is not None
             and plot_cluster_name != "label"
             and plot_cluster_name in list(features.keys())
         ):
             if self.plot_hide_non_selected.isChecked():
                 features.loc[
                     features[plot_cluster_name] == 0, plot_cluster_name
                 ] = -1  # make unselected points to noise points
+
             # fill all prediction nan values with -1 -> turns them
             # into noise points
             self.label_ids = features["label"]
             self.cluster_ids = features[plot_cluster_name].fillna(-1)
 
-            # get long colormap from function
-            colors = get_nice_colormap()
             if len(self.analysed_layer.data.shape) == 4 and not tracking_data:
                 frame_id = features[POINTER].tolist()
                 current_frame = self.frame
             elif len(self.analysed_layer.data.shape) <= 3 or tracking_data:
                 frame_id = None
                 current_frame = None
             else:
                 warnings.warn("Image dimensions too high for processing!")
 
-            a, sizes, colors_plot = clustered_plot_parameters(
-                cluster_id=self.cluster_ids,
-                frame_id=frame_id,
-                current_frame=current_frame,
-                n_datapoints=number_of_points,
-                color_hex_list=colors,
-            )
+            if self.plotting_type.currentText() == PlottingType.SCATTER.name:
+                a, sizes, colors_plot = clustered_plot_parameters(
+                    cluster_id=self.cluster_ids,
+                    frame_id=frame_id,
+                    current_frame=current_frame,
+                    n_datapoints=number_of_points,
+                    color_hex_list=colors,
+                )
 
-            self.graphics_widget.pts = self.graphics_widget.axes.scatter(
-                self.data_x,
-                self.data_y,
-                c=colors_plot,
-                s=sizes,
-                alpha=a,
-            )
-            self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
-            self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
-            self.graphics_widget.match_napari_layout()
+                self.graphics_widget.make_scatter_plot(
+                    self.data_x, self.data_y, colors_plot, sizes, a
+                )
 
-            # Here canvas is drawn
-            self.graphics_widget.selector.disconnect()
-            self.graphics_widget.selector = SelectFromCollection(
-                self.graphics_widget,
-                self.graphics_widget.axes,
-                self.graphics_widget.pts,
-            )
+                self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
+            else:
+                if self.bin_auto.isChecked():
+                    if plot_x_axis_name == plot_y_axis_name:
+                        number_bins = int(estimate_number_bins(self.data_x))
+                    else:
+                        number_bins = int(
+                            np.max(
+                                [
+                                    estimate_number_bins(self.data_x),
+                                    estimate_number_bins(self.data_y),
+                                ]
+                            )
+                        )
+                        self.bin_number_spinner.setValue(number_bins)
+                else:
+                    number_bins = int(self.bin_number_spinner.value())
+
+                # if both axes are the same, plot 1D histogram
+                if plot_x_axis_name == plot_y_axis_name:
+                    self.graphics_widget.make_1d_histogram(
+                        self.data_x,
+                        bin_number=number_bins,
+                        log_scale=self.log_scale.isChecked(),
+                    )
+                    # update bar colors to cluster ids
+                    self.graphics_widget.axes = apply_cluster_colors_to_bars(
+                        self.graphics_widget.axes,
+                        cluster_name=plot_cluster_name,
+                        features=features,
+                        number_bins=number_bins,
+                        feature_x=self.plot_x_axis_name,
+                        colors=colors,
+                    )
+                    self.graphics_widget.figure.canvas.draw_idle()
+                    self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                    self.graphics_widget.axes.set_ylabel("frequency")
+                else:
+                    self.graphics_widget.make_2d_histogram(
+                        self.data_x,
+                        self.data_y,
+                        colors,
+                        bin_number=number_bins,
+                        log_scale=self.log_scale.isChecked(),
+                    )
+
+                    rgb_img = make_cluster_overlay_img(
+                        cluster_id=plot_cluster_name,
+                        features=features,
+                        feature_x=self.plot_x_axis_name,
+                        feature_y=self.plot_y_axis_name,
+                        colors=colors,
+                        histogram_data=self.graphics_widget.histogram,
+                        hide_first_cluster=self.plot_hide_non_selected.isChecked(),
+                    )
+                    xedges = self.graphics_widget.histogram[1]
+                    yedges = self.graphics_widget.histogram[2]
+
+                    self.graphics_widget.axes.imshow(
+                        rgb_img,
+                        extent=[xedges[0], xedges[-1], yedges[0], yedges[-1]],
+                        origin="lower",
+                        alpha=1,
+                        aspect="auto",
+                    )
+                    self.graphics_widget.figure.canvas.draw_idle()
+                    self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                    self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
+
+            self.graphics_widget.match_napari_layout()
 
             from vispy.color import Color
 
             cmap = [Color(hex_name).RGBA.astype("float") / 255 for hex_name in colors]
 
             # generate dictionary mapping each prediction to its respective color
             # list cycling with  % introduced for all labels except hdbscan noise points (id = -1)
@@ -506,32 +732,61 @@
                 current_frame = self.frame
             elif len(self.analysed_layer.data.shape) <= 3 or tracking_data:
                 frame_id = None
                 current_frame = None
             else:
                 warnings.warn("Image dimensions too high for processing!")
 
-            a, sizes, colors_plot = unclustered_plot_parameters(
-                frame_id=frame_id,
-                current_frame=current_frame,
-                n_datapoints=number_of_points,
-            )
+            if self.plotting_type.currentText() == PlottingType.SCATTER.name:
+                a, sizes, colors_plot = unclustered_plot_parameters(
+                    frame_id=frame_id,
+                    current_frame=current_frame,
+                    n_datapoints=number_of_points,
+                )
 
-            self.graphics_widget.pts = self.graphics_widget.axes.scatter(
-                self.data_x,
-                self.data_y,
-                color=colors_plot,
-                s=sizes,
-                alpha=a,
-            )
-            self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
-            self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
-            self.graphics_widget.match_napari_layout()
+                self.graphics_widget.make_scatter_plot(
+                    self.data_x, self.data_y, colors_plot, sizes, a
+                )
 
-            self.graphics_widget.selector = SelectFromCollection(
-                self.graphics_widget,
-                self.graphics_widget.axes,
-                self.graphics_widget.pts,
-            )
+                self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
+            else:
+                if self.bin_auto.isChecked():
+                    if plot_x_axis_name == plot_y_axis_name:
+                        number_bins = int(estimate_number_bins(self.data_x))
+                    else:
+                        number_bins = int(
+                            np.max(
+                                [
+                                    estimate_number_bins(self.data_x),
+                                    estimate_number_bins(self.data_y),
+                                ]
+                            )
+                        )
+                    self.bin_number_spinner.setValue(number_bins)
+                else:
+                    number_bins = int(self.bin_number_spinner.value())
+
+                # if both axes are the same, plot 1D histogram
+                if plot_x_axis_name == plot_y_axis_name:
+                    self.graphics_widget.make_1d_histogram(
+                        self.data_x,
+                        bin_number=number_bins,
+                        log_scale=self.log_scale.isChecked(),
+                    )
+                    self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                    self.graphics_widget.axes.set_ylabel("frequency")
+                else:
+                    self.graphics_widget.make_2d_histogram(
+                        self.data_x,
+                        self.data_y,
+                        colors,
+                        bin_number=number_bins,
+                        log_scale=self.log_scale.isChecked(),
+                    )
+                    self.graphics_widget.axes.set_xlabel(plot_x_axis_name)
+                    self.graphics_widget.axes.set_ylabel(plot_y_axis_name)
+
+            self.graphics_widget.match_napari_layout()
 
-            self.graphics_widget.draw()  # Only redraws when cluster is not manually selected
-            # because manual selection already does that when selector is disconnected
+        self.graphics_widget.draw()  # Always redraws, oterwise y-axis may not get updated in histograms
+        self.graphics_widget.reset_zoom()
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_clustering.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_dimension_reduction.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dimension_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sys
 
 import numpy as np
 import pandas as pd
 from skimage import measure
 
+from napari_clusters_plotter._utilities import get_layer_tabular_data
+
 sys.path.append("../")
 
 
 def test_clustering_widget(make_napari_viewer):
     import napari_clusters_plotter as ncp
 
     viewer = make_napari_viewer(strict_qt=True)
@@ -69,19 +71,23 @@
         explained_variance=95.0,
         pca_components=0,
         mds_metric=True,
         mds_n_init=4,
         mds_max_iter=300,
         mds_eps=0.001,
         umap_multithreading=True,
+        min_dist=0.1,
+        custom_name="",
     )
 
     blocker = qtbot.waitSignal(widget.worker.finished, timeout=1000000)
     blocker.wait()
 
+    assert "UMAP_0" in get_layer_tabular_data(labels_layer)
+
 
 """
 def test_call_to_function(qtbot, make_napari_viewer):
 
     viewer = make_napari_viewer(strict_qt=True)
 
     label = np.array(
@@ -177,15 +183,17 @@
 def test_umap():
     from napari_clusters_plotter._dimensionality_reduction import umap
 
     X = np.array([[0, 0, 0], [0, 1, 1], [1, 0, 1], [1, 1, 1]])
     nr_components = 2
 
     # umap returns (str, np.ndarray), where the first item is algorithm name
-    result = umap(pd.DataFrame(X), n_neighbors=2, n_components=nr_components)
+    result = umap(
+        pd.DataFrame(X), n_neighbors=2, n_components=nr_components, min_dist=0.1
+    )
 
     assert result[1].shape[-1] == nr_components
 
 
 def test_tsne():
     from napari_clusters_plotter._dimensionality_reduction import tsne
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_dock_widget.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_plotter.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_plotter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 from skimage import measure
 
 import napari_clusters_plotter as ncp
 from napari_clusters_plotter._plotter_utilities import (
     alpha_factor,
     alphas_clustered,
     alphas_unclustered,
@@ -16,53 +17,49 @@
     spot_size_clustered,
     spot_size_unclustered,
     unclustered_plot_parameters,
 )
 from napari_clusters_plotter._utilities import get_layer_tabular_data, get_nice_colormap
 
 
-def test_plotting(make_napari_viewer):
-    viewer = make_napari_viewer()
-    widget_list = ncp.napari_experimental_provide_dock_widget()
-
+def get_labels_array():
     label = np.array(
         [
             [0, 0, 0, 0, 0, 0, 0],
             [0, 1, 1, 0, 0, 2, 2],
             [0, 0, 0, 0, 2, 2, 2],
             [3, 3, 0, 0, 0, 0, 0],
             [0, 0, 4, 4, 0, 5, 5],
             [6, 6, 6, 6, 0, 5, 0],
             [0, 7, 7, 0, 0, 0, 0],
         ]
     )
+    return label
+
+
+def test_plotting(make_napari_viewer):
+    viewer = make_napari_viewer()
+    widget_list = ncp.napari_experimental_provide_dock_widget()
 
-    # image = label * 1.5
+    label = get_labels_array()
 
     props = measure.regionprops_table(
         label, properties=(["label", "area", "perimeter"])
     )
 
     label_layer = viewer.add_labels(label, properties=props)
-    # image_layer = viewer.add_image(image)
 
     for widget in widget_list:
         _widget = widget(viewer)
-        # Doesn't work for now to use in tests because MeasureWidget uses cle function
-        # if isinstance(_widget, ncp._measure.MeasureWidget):
-        #     _widget.run(
-        #         image_layer, label_layer, "Measure now intensity shape", None, None
-        #     )
 
         if isinstance(_widget, ncp._plotter.PlotterWidget):
             plot_widget = _widget
 
     viewer.window.add_dock_widget(plot_widget)
     assert len(viewer.window._dock_widgets) == 1
-    # assert len(viewer.window._dock_widgets) == 2
 
     result = get_layer_tabular_data(label_layer)
 
     assert "label" in result.columns
     assert "area" in result.columns
     assert "perimeter" in result.columns
 
@@ -120,15 +117,15 @@
     ]
 
     assert spots_unclustered == result_su
 
     colors_cl = colors_clustered(predicts, frame_ids, current_frame, colors)
     result = [colors[pred] if pred >= 0 else "#bcbcbc" for pred in predicts]
     result_cc = [
-        result[i] if frame != current_frame else highlight
+        result[i] if frame != current_frame else gen_highlight(result[i])
         for i, frame in enumerate(frame_ids)
     ]
 
     assert colors_cl == result_cc
 
     colors_uc = colors_unclustered(frame_ids, current_frame)
     result_cu = [
@@ -141,7 +138,73 @@
     cl_plot_params = clustered_plot_parameters(
         predicts, frame_ids, current_frame, n_datapoints, colors
     )
     assert cl_plot_params == (result_ac, result_sc, result_cc)
 
     uc_plot_params = unclustered_plot_parameters(frame_ids, current_frame, n_datapoints)
     assert uc_plot_params == (result_au, result_su, result_cu)
+
+
+def test_plotting_histogram(make_napari_viewer):
+    from napari_clusters_plotter._plotter import PlotterWidget
+
+    viewer = make_napari_viewer()
+
+    label = get_labels_array()
+    measurements = measure.regionprops_table(
+        label, properties=(["label", "area", "perimeter"])
+    )
+    label_layer = viewer.add_labels(label, properties=measurements)
+    label_layer.features = measurements
+
+    viewer.window.add_dock_widget(PlotterWidget(viewer), area="right")
+    plotter_widget = PlotterWidget(viewer)
+    plotter_widget.plotting_type.setCurrentText("HISTOGRAM_2D")
+
+    plotter_widget.run(
+        features=pd.DataFrame(measurements),
+        plot_x_axis_name="area",
+        plot_y_axis_name="perimeter",
+        force_redraw=True,
+    )
+
+    assert plotter_widget.graphics_widget.axes.has_data()
+
+    # test plotting 1D histogram
+    plotter_widget.run(
+        features=pd.DataFrame(measurements),
+        plot_x_axis_name="area",
+        plot_y_axis_name="area",
+        force_redraw=True,
+    )
+
+    assert plotter_widget.graphics_widget.axes.has_data()
+
+
+def test_cluster_image_generation_for_histogram(make_napari_viewer):
+    from napari_clusters_plotter._plotter import PlotterWidget
+
+    viewer = make_napari_viewer()
+
+    label = get_labels_array()
+    measurements = measure.regionprops_table(
+        label, properties=(["label", "area", "perimeter"])
+    )
+    measurements["MANUAL_CLUSTER_ID"] = np.array([1, 0, 2, -1, 0, 1, 2])
+    viewer.add_labels(label, properties=measurements)
+
+    viewer.window.add_dock_widget(PlotterWidget(viewer), area="right")
+    plotter_widget = PlotterWidget(viewer)
+    plotter_widget.plotting_type.setCurrentText("HISTOGRAM_2D")
+    plotter_widget.log_scale.value = True
+
+    plotter_widget.run(
+        features=pd.DataFrame(measurements),
+        plot_x_axis_name="area",
+        plot_y_axis_name="perimeter",
+        plot_cluster_name="MANUAL_CLUSTER_ID",
+        force_redraw=True,
+    )
+
+    assert plotter_widget.graphics_widget.axes.has_data()
+    assert "cluster_ids_in_space" in viewer.layers
+    assert int(viewer.layers["cluster_ids_in_space"].data.max()) == 3
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_tests/test_utils.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/_utilities.py` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,17 @@
 
     # reforming the prediction list, this is done to account
     # for cluster labels that start at 0, conveniently hdbscan
     # labelling starts at -1 for noise, removing these from the labels
     predictionlist_new = np.array(predictionlist) + 1
     label_list = np.array(label_list)
 
-    return map_array(label_image, label_list, predictionlist_new).astype("uint64")
+    return map_array(np.asarray(label_image), label_list, predictionlist_new).astype(
+        "uint64"
+    )
 
 
 def dask_cluster_image_timelapse(label_image, label_id_list, prediction_list_list):
     """
     Generates a timelapse of cluster images using Dask.
 
     Given a label image and a list of prediction lists, this function generates a timelapse
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Back.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Back.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Customize.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Customize.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Forward.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Forward.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Home.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Home.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Pan.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Pan_checked.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Save.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Save.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Subplots.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Zoom.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter/icons/Zoom_checked.png` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/PKG-INFO` & `napari-clusters-plotter-0.7.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,21 @@
-Metadata-Version: 2.1
-Name: napari-clusters-plotter
-Version: 0.6.2
-Summary: A plugin to use with napari for clustering objects according to their properties
-Home-page: https://github.com/BiAPoL/napari-clusters-plotter
-Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
-Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
-Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
-Project-URL: Source Code, https://github.com/BiAPoL/napari-clusters-plotter
-Project-URL: User Support, https://github.com/BiAPoL/napari-clusters-plotter/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # napari-clusters-plotter
 
 [![License](https://img.shields.io/pypi/l/napari-clusters-plotter.svg?color=green)](https://github.com/lazigu/napari-clusters-plotter/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-clusters-plotter.svg?color=green)](https://pypi.org/project/napari-clusters-plotter)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-clusters-plotter.svg?color=green)](https://python.org)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/version.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
-[![tests](https://github.com/lazigu/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/lazigu/napari-clusters-plotter/actions)
+[![tests](https://github.com/BiAPoL/napari-clusters-plotter/workflows/tests/badge.svg)](https://github.com/BiAPoL/napari-clusters-plotter/actions)
 [![codecov](https://codecov.io/gh/BiAPoL/napari-clusters-plotter/branch/main/graph/badge.svg?token=R6W2KO1NJ8)](https://codecov.io/gh/BiAPoL/napari-clusters-plotter)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/napari-clusters-plotter/badges/downloads.svg)](https://anaconda.org/conda-forge/napari-clusters-plotter)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-clusters-plotter)](https://www.napari-hub.org/plugins/napari-clusters-plotter)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7011471.svg)](https://doi.org/10.5281/zenodo.7011471)
 
-A plugin to use with napari for clustering objects according to their properties.
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
-<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
-
-Demonstration of handling 3D time-lapse data:
+A napari-plugin for clustering objects according to their properties.
 
 <img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast2_timelapse.gif" width="700"/>
 
 ----------------------------------
 
 Jump to:
 - [Usage](#usage)
@@ -76,253 +40,176 @@
 For clustering objects according to their properties, the starting point is a [grey-value image](example_data/blobs.tif) and a label image
 representing a segmentation of objects. For segmenting objects, you can for example use the
 [Voronoi-Otsu-labelling approach](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes#voronoi-otsu-labelling)
 in the napari plugin [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/starting_point.png)
 
-### Measurements
-The first step is deriving measurements from the labelled image and the corresponding pixels in the grey-value image.
-Since the 0.6.0 release measurements widget is no longer part of this plugin and you will have to use other napari plugins to measure your data.
-One way is to use the measurement functions in [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops), which comes pre-installed with the napari cluster plotter.
-Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget.
-Just select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-In the previous napari-cluster-plotter release a GPU dependant measurement function was implemented which you can find in the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-To use this function you will need to install this library (see optional installation steps) and you can find the widget under the menu `Tools > Measurement tables > Label statistics (clEsperanto)`. As before, select the image, the corresponding label image and the measurements to analyse and click on `Run`.
-
-A table with the measurements will open and afterwards, you can save and/or close the measurement table. Also, close the Measure widget.
-
-If you want to upload your own measurements you can do this using [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops).
-Under the menu `Tools > Measurement tables > Load from CSV (nsr)` you can find a widget to upload your own csv file.
-Make sure that there is a column that specifies the which measurement belongs to which label by adding a column with the name "label".
-If you don't specify this column it will be assumed that measurements start at 1 and each
-column describes the next label.
-
-Note that tables for time-lapse data need to include an **additional column named "frame"**, which indicates which slice in
-time the given row refers to.
-
-**For the correct visualisation of clusters IDs in space**, it is **important** that label images/time-points of the time-lapse
-are either **labelled sequentially** or missing labels still exist in the loaded csv file (i.e., missing label exists in the
-"label" column with `NaN` values for other measurements in the same row). If you perform measurements using before mentioned
-plugins, the obtained dataframe is already in the correct form.
-
-#### Time-Lapse Measurements
-In case you have 2D time-lapse data you need to convert it into a suitable shape using the function: `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)`,
-which can be found in the [napari time slicer](https://www.napari-hub.org/plugins/napari-time-slicer).
-
-Note that tables for time-lapse data will include an additional column named "frame", which indicates which slice in
-time the given row refers to. If you want to import your own csv files for time-lapse data make sure to include this column!
-If you have tracking data where each column specifies measurements for a track instead of a label at a specific time point,
-this column must not be added.
+In case you have 2D time-lapse data you need to convert it into a suitable shape using the menu `Tools > Utilities > Convert 3D stack to 2D time-lapse (time-slicer)` ([documentation](https://www.napari-hub.org/plugins/napari-time-slicer)).
 
-Both [napari-skimage-regionprops](https://www.napari-hub.org/plugins/napari-skimage-regionprops) and [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant) include measuring widgets for timelapse data.
+### Measurements
+The first step is deriving measurements from the labeled image and the corresponding pixels in the grey-value image. 
+Use the menu `Tools > Measurement tables > Regionprops (scikit-image, nsr)` to get to the measurement widget ([documentation](https://www.napari-hub.org/plugins/napari-skimage-regionprops)).
+Select the image, the corresponding label image and the measurements to analyse and click on `Run`.
+A table with the measurements will open and afterwards, you can save and/or close the measurement table. 
+At this point it is recommended to close the table and the Measure widget to free space for following steps.
+
+You can also load your own measurements you can do this using the menu `Tools > Measurement tables > Load from CSV (nsr)`.
+If you load custom measurements, please make sure that there is a `label` column that specifies the which measurement belongs to which labeled object.
+Tables for time-lapse data need to include an additional column named `frame`.
 
 ### Plotting
 
-Once measurements were made or uploaded, these measurements were saved in the `properties/features` of the labels layer which was
-analysed. You can then plot these measurements using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
+Once measurements were saved in the labels layer which was analysed, you can then plot these measurements using the menu `Tools > Visualization > Plot measurements (ncp)`.
 
 In this widget, you can select the labels layer which was analysed and the measurements which should be plotted
-on the X- and Y-axis. If you cannot see any options in axes selection boxes, but you have performed measurements, click
-on `Update Axes/Clustering Selection Boxes` to refresh them. Click on `Run` to draw the data points in the plot area.
+on the X- and Y-axis. Click on `Plot` to draw the data points in the plot area.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_plain.png)
 
-You can also manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
+Under advanced options, you can also select the plot type histogram which will visualize a 2D histogram. 2D histogram visualization is recommended if you have a very high number of data points.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_2d.png)
+
+If you choose the same measurement for the X and the Y axis, a histogram will be shown.
+
+![img.png](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/histogram_1d.png)
+
+Under advanced options you will also find the checkbox determining whether not-selected data points should be hidden (shown in grey) or automatically
+clustered as another cluster.
+
+### Manual clustering
+
+You can manually select a region in the plot. To use lasso (freehand) tool use left mouse click, and to use a
 rectangle - right click. The resulting manual clustering will also be visualized in the original image. To optimize
 visualization in the image, turn off the visibility of the analysed labels layer.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plot_interactive.png)
+<img src="https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/screencast.gif" width="700"/>
 
 Hold down the SHIFT key while annotating regions in the plot to manually select multiple clusters.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/multi-select-manual-clustering.gif)
 
-#### Time-Lapse Plotting
+### Saving manual clustering
+
+Manual clustering results can be saved by going to `Tools > Measurement > Show table (nsr)`, and clicking on `Save as csv`.
+The saved table will contain a "MANUAL_CLUSTER_ID" column. This column is overwritten every time different clusters are manually selected.
+
+### Time-Lapse analysis
+
 When you plot your time-lapse datasets you will notice that the plots look slightly different.
-Datapoints of the current time frame are highlighted in white and you can see the datapoints move through the plot if you press play:
+Datapoints of the current time frame are highlighted in bright color and you can see the datapoints move through the plot while you navigate through time:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/plotting_time-lapse_data_as_movie.gif)
 
 You can also manually select groups using the lasso tool and plot a measurement per frame and see how the group behaves in time.
 Furthermore, you could also select a group in time and see where the datapoints lie in a different feature space:
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/timelapse_manual_clustering_tips.gif)
 
-### Dimensionality reduction: UMAP, t-SNE or PCA
+If you have custom measurements from tracking data where each column specifies measurements for a track instead of a label at a specific time point, the `frame` column must not be added.
+
+### Dimensionality reduction
 
-For getting more insights into your data, you can reduce the dimensionality of the measurements, e.g.
-using the [UMAP algorithm](https://umap-learn.readthedocs.io/en/latest/), [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
-or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html).
-To apply it to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
-Select the label image that was analysed and in the list below, select all measurements that should be
-dimensionality reduced. By default, all measurements are selected in the box. If you cannot see any measurements, but
-you have performed them, click on `Update Measurements` to refresh the box. You can read more about parameters of both
-algorithms by hovering over question marks or by clicking on them. When you are done with the selection, click on `Run`
-and after a moment, the table of measurements will re-appear with two additional columns representing the reduced
-dimensions of the dataset. These columns are automatically saved in the `properties` of the labels layer so there is no
-need to save them for usage in other widgets unless you wish to do so.
+For getting more insights into your data, you can reduce the dimensionality of the measurements, using these algorithms:
+* [Uniform Manifold Approximation Projection (UMAP)](https://umap-learn.readthedocs.io/en/latest/)
+* [t-distributed stochastic neighbor embedding (t-SNE)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)
+* [Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
+* [Non-linear dimensionality reduction through Isometric Mapping (Isomap)](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.Isomap.html)
+* [Multi-dimensional Scaling (MDS)](https://scikit-learn.org/stable/modules/manifold.html#multidimensional-scaling)
+
+To apply them to your data use the menu `Tools > Measurement post-processing > Dimensionality reduction (ncp)`.
+Select the label image that was analysed and in the list below, select all measurements that should be dimensionality reduced. 
+By default, all measurements are selected in the box. 
+You can read more about parameters of both algorithms by hovering over question marks or by clicking on them. 
+When you are done with the selection, click on `Run` and after a moment, the table of measurements will re-appear with two additional columns representing the reduced dimensions of the dataset. 
+These columns are automatically saved in the labels layer and can be further processed by other plugins.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/umap.png)
 
-Afterwards, you can again save and/or close the table. Also, close the Dimensionality Reduction widget.
+Afterwards, you can again save and/or close the table.
 
 ### Clustering
 If manual clustering, as shown above, is not an option, you can automatically cluster your data, using these implemented algorithms:
 * [k-means clustering (KMEANS)](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)
 * [Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN)](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
 * [Gaussian Mixture Model (GMM)](https://scikit-learn.org/stable/modules/mixture.html)
 * [Mean Shift (MS)](https://scikit-learn.org/stable/auto_examples/cluster/plot_mean_shift.html#sphx-glr-auto-examples-cluster-plot-mean-shift-py)
 * [Agglomerative clustering (AC)](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
 
-Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`,
-again, select the analysed labels layer.
-This time select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
+Therefore, click the menu `Tools > Measurement post-processing > Clustering (ncp)`, 
+select the analysed labels layer.
+Select the measurements for clustering, e.g. select _only_ the `UMAP` measurements.
 Select the clustering method `KMeans` and click on `Run`.
 The table of measurements will reappear with an additional column `ALGORITHM_NAME_CLUSTERING_ID` containing the cluster
 ID of each datapoint.
 
 ![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/clustering.png)
 
-Afterwards, you can again save and/or close the table. Also, close the clustering widget.
+Afterwards, you can save and/or close the table.
 
 ### Plotting clustering results
-Return to the Plotter widget using the menu `Tools > Measurement tables > Plot measurement (ncp)`.
-Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Run`.
-
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
 
-Example of k-means clustering results:
+Return to the Plotter widget using the menu `Tools > Visualization > Plot measurement (ncp)`.
+Select `UMAP_0` and `UMAP_1` as X- and Y-axis and the `ALGORITHM_NAME_CLUSTERING_ID` as `Clustering`, and click on `Plot`.
 
-![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/kmeans_clusters_plot.png)
+![](https://github.com/BiAPoL/napari-clusters-plotter/raw/main/images/hdbscan_clusters_plot.png)
 
 ## Installation
 ### Devbio-napari installation
-The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) library.
-This library installs napari alongside many other useful plugins, including the napari-clusters-plotter.
-We recommend this library as it is not only the easiest way to install the napari-cluster-plotter, but it includes plugins for segmentation and measurement, which we don't provide.
-There are detailed installation instructions on the [napari-hub-page](https://www.napari-hub.org/plugins/devbio-napari) if you have any problems installing it.
-In case you want to have a minimal installation of our plugin you can find other installation options below.
+
+The easiest way to install this plugin is to install the [devbio-napari](https://github.com/haesleinhuepf/devbio-napari) plugin collection. The napari-clusters-plotter is part of it.
 
 ### Minimal installation
 * Get a python environment, e.g. via [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
-  If you never used python/conda environments before, please follow the instructions
-  [here](https://mpicbg-scicomp.github.io/ipf_howtoguides/guides/Python_Conda_Environments) first. It is recommended to
-  install python 3.9 to your new conda environment from the start. The plugin is not yet supported with Python 3.10.
-  Create a new environment, for example, like this:
-
-```
-conda create --name ncp-env python=3.9
-```
-
-* Activate the new environment via conda:
-
-```
-conda activate ncp-env
-```
-
-* Install [napari], e.g. via [conda]:
+  If you never used mamba/conda environments before, please follow the instructions
+  [in this blog post](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html) first. 
 
-```
-conda install -c conda-forge napari
-```
-
-Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
+* Create a new environment, for example, like this:
 
 ```
-conda install -c conda-forge napari-clusters-plotter
+mamba create --name ncp-env python=3.9
 ```
 
-### Optional installation
-Follow these steps instead of the regular installation to include the [napari-pyclesperanto-assistant](https://www.napari-hub.org/plugins/napari-pyclesperanto-assistant).
-Creating the environment like this will allow you to use your GPU to render your cluster results.
-Furthermore, you can access the deprecated measurement functions of the napari-cluster-plotter in releases < 0.6.0.
-If you have trouble with this library you can use the regular installation above.
-
-```
-conda create --name ncp-env python==3.9
-```
-
-
 * Activate the new environment via conda:
 
 ```
-conda activate ncp-env
-```
-
-* Install napari-pyclesperanto-assistant, e.g. with pip:
-
-```
-pip install napari-pyclesperanto-assistant
-```
-
-* Mac-users please also install this:
-
-```
-conda install -c conda-forge ocl_icd_wrapper_apple
+mamba activate ncp-env
 ```
 
-* Linux users please also install this:
+* Install [napari], e.g. via [conda]:
 
 ```
-conda install -c conda-forge ocl-icd-system
-```
-
-* Install [napari], e.g. via [pip] or [conda]:
-
-```
-python -m pip install "napari[all]"
-```
-```
-conda install -c conda-forge napari
+mamba install -c conda-forge napari
 ```
 
 Afterwards, you can install `napari-clusters-plotter`, e.g. via [conda]:
 
 ```
-conda install -c conda-forge napari-clusters-plotter
+mamba install -c conda-forge napari-clusters-plotter
 ```
 
 ## Troubleshooting installation
 
-- If the plugin does not appear in napari 'Plugins' menu, and in 'Plugin errors...' you can see such an error:
-
-```
-ImportError: DLL load failed while importing _cl
-```
-
-Try downloading and installing a pyopencl with a lower cl version, e.g. cl12 : pyopencl=2020.1. However, in this case,
-you will need an environment with a lower python version (python=3.8).
-
 - `Error: Could not build wheels for hdbscan which use PEP 517 and cannot be installed directly`
 
 This can happen if you used pip for the installation. To solve this error, install hdbscan via conda before installing the plugin:
 
 ```
-conda install -c conda-forge hdbscan
+mamba install -c conda-forge hdbscan
 ```
 
 - `ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 96 from C header, got 88 from PyObject`
 
 Similar to the above-described error, this error can occur when importing hdbscan through pip or in the wrong order. This can be fixed by installing packages separately through conda and in the following order:
 ```bash
-conda install -c conda-forge napari pyopencl hdbscan
+mamba install -c conda-forge napari hdbscan
 pip install napari-clusters-plotter
 ```
 
-- `WARNING: No ICDs were found` or `LogicError: clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR`
-
-Make your system-wide implementation visible by installing either of the following conda packages:
-
-```
-conda install -c conda-forge ocl-icd-system
-conda install -c conda-forge ocl_icd_wrapper_apple
-```
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [pytest], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-clusters-plotter-0.6.2/napari_clusters_plotter.egg-info/SOURCES.txt` & `napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/requirements.txt` & `napari-clusters-plotter-0.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.6.2/setup.cfg` & `napari-clusters-plotter-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 636c 7573 7465   = napari-cluste
 00000020: 7273 2d70 6c6f 7474 6572 0d0a 7665 7273  rs-plotter..vers
-00000030: 696f 6e20 3d20 302e 362e 320d 0a61 7574  ion = 0.6.2..aut
+00000030: 696f 6e20 3d20 302e 372e 300d 0a61 7574  ion = 0.7.0..aut
 00000040: 686f 7220 3d20 4c61 7572 6120 5a69 6775  hor = Laura Zigu
 00000050: 7479 7465 2c20 5279 616e 2053 6176 696c  tyte, Ryan Savil
 00000060: 6c2c 204a 6f68 616e 6e65 7320 4dc3 bc6c  l, Johannes M..l
 00000070: 6c65 722c 204d 6172 6365 6c6f 205a 6f63  ler, Marcelo Zoc
 00000080: 636f 6c65 722c 2052 6f62 6572 7420 4861  coler, Robert Ha
 00000090: 6173 650d 0a61 7574 686f 725f 656d 6169  ase..author_emai
 000000a0: 6c20 3d20 7a69 6775 7479 7465 4067 6d61  l = zigutyte@gma
@@ -78,43 +78,44 @@
 000004d0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
 000004e0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 000004f0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 00000500: 3d20 3e3d 332e 370d 0a69 6e73 7461 6c6c  = >=3.7..install
 00000510: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
 00000520: 6170 6172 692d 706c 7567 696e 2d65 6e67  apari-plugin-eng
 00000530: 696e 653e 3d30 2e31 2e34 0d0a 096e 756d  ine>=0.1.4...num
-00000540: 7079 3e3d 312e 3231 0d0a 0973 6369 6b69  py>=1.21...sciki
-00000550: 742d 6c65 6172 6e0d 0a09 6d61 7470 6c6f  t-learn...matplo
-00000560: 746c 6962 0d0a 0970 616e 6461 730d 0a09  tlib...pandas...
-00000570: 756d 6170 2d6c 6561 726e 0d0a 096e 6170  umap-learn...nap
-00000580: 6172 692d 746f 6f6c 732d 6d65 6e75 0d0a  ari-tools-menu..
-00000590: 096e 6170 6172 692d 736b 696d 6167 652d  .napari-skimage-
-000005a0: 7265 6769 6f6e 7072 6f70 733e 3d30 2e33  regionprops>=0.3
-000005b0: 2e31 0d0a 0968 6462 7363 616e 0d0a 096a  .1...hdbscan...j
-000005c0: 6f62 6c69 620d 0a0d 0a5b 6f70 7469 6f6e  oblib....[option
-000005d0: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
-000005e0: 0a6e 6170 6172 692e 706c 7567 696e 203d  .napari.plugin =
-000005f0: 200d 0a09 6e61 7061 7269 2d63 6c75 7374   ...napari-clust
-00000600: 6572 732d 706c 6f74 7465 7220 3d20 6e61  ers-plotter = na
-00000610: 7061 7269 5f63 6c75 7374 6572 735f 706c  pari_clusters_pl
-00000620: 6f74 7465 720d 0a0d 0a5b 666c 616b 6538  otter....[flake8
-00000630: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
-00000640: 7468 203d 2031 3230 0d0a 6967 6e6f 7265  th = 120..ignore
-00000650: 203d 2045 3230 332c 5735 3033 2c43 3930   = E203,W503,C90
-00000660: 312c 4638 3233 0d0a 6d61 782d 636f 6d70  1,F823..max-comp
-00000670: 6c65 7869 7479 203d 2031 380d 0a62 7569  lexity = 18..bui
-00000680: 6c74 696e 7320 3d20 7079 7465 7374 0d0a  ltins = pytest..
-00000690: 6578 636c 7564 6520 3d20 6e61 7061 7269  exclude = napari
-000006a0: 5f63 6c75 7374 6572 735f 706c 6f74 7465  _clusters_plotte
-000006b0: 722f 5f5f 696e 6974 5f5f 2e70 792c 2065  r/__init__.py, e
-000006c0: 7861 6d70 6c65 5f64 6174 612c 2069 6d61  xample_data, ima
-000006d0: 6765 732c 206e 6170 6172 695f 636c 7573  ges, napari_clus
-000006e0: 7465 7273 5f70 6c6f 7474 6572 2f5f 6765  ters_plotter/_ge
-000006f0: 745f 636f 6c6f 726d 6170 2e70 790d 0a62  t_colormap.py..b
-00000700: 616e 6e65 642d 6d6f 6475 6c65 7320 3d20  anned-modules = 
-00000710: 5079 5174 3520 3d20 7573 6520 7174 7079  PyQt5 = use qtpy
-00000720: 0d0a 0950 7953 6964 6532 203d 2075 7365  ...PySide2 = use
-00000730: 2071 7470 790d 0a0d 0a5b 6973 6f72 745d   qtpy....[isort]
-00000740: 0d0a 7072 6f66 696c 6520 3d20 626c 6163  ..profile = blac
-00000750: 6b0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  k....[egg_info].
-00000760: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000770: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000540: 7079 3e3d 312e 3231 2c3c 3d31 2e32 332e  py>=1.21,<=1.23.
+00000550: 350d 0a09 7363 696b 6974 2d6c 6561 726e  5...scikit-learn
+00000560: 0d0a 096d 6174 706c 6f74 6c69 620d 0a09  ...matplotlib...
+00000570: 7061 6e64 6173 0d0a 0975 6d61 702d 6c65  pandas...umap-le
+00000580: 6172 6e0d 0a09 6e61 7061 7269 2d74 6f6f  arn...napari-too
+00000590: 6c73 2d6d 656e 750d 0a09 6e61 7061 7269  ls-menu...napari
+000005a0: 2d73 6b69 6d61 6765 2d72 6567 696f 6e70  -skimage-regionp
+000005b0: 726f 7073 3e3d 302e 332e 310d 0a09 6864  rops>=0.3.1...hd
+000005c0: 6273 6361 6e0d 0a09 6a6f 626c 6962 0d0a  bscan...joblib..
+000005d0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+000005e0: 5f70 6f69 6e74 735d 0d0a 6e61 7061 7269  _points]..napari
+000005f0: 2e70 6c75 6769 6e20 3d20 0d0a 096e 6170  .plugin = ...nap
+00000600: 6172 692d 636c 7573 7465 7273 2d70 6c6f  ari-clusters-plo
+00000610: 7474 6572 203d 206e 6170 6172 695f 636c  tter = napari_cl
+00000620: 7573 7465 7273 5f70 6c6f 7474 6572 0d0a  usters_plotter..
+00000630: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
+00000640: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
+00000650: 300d 0a69 676e 6f72 6520 3d20 4532 3033  0..ignore = E203
+00000660: 2c57 3530 332c 4339 3031 2c46 3832 330d  ,W503,C901,F823.
+00000670: 0a6d 6178 2d63 6f6d 706c 6578 6974 7920  .max-complexity 
+00000680: 3d20 3138 0d0a 6275 696c 7469 6e73 203d  = 18..builtins =
+00000690: 2070 7974 6573 740d 0a65 7863 6c75 6465   pytest..exclude
+000006a0: 203d 206e 6170 6172 695f 636c 7573 7465   = napari_cluste
+000006b0: 7273 5f70 6c6f 7474 6572 2f5f 5f69 6e69  rs_plotter/__ini
+000006c0: 745f 5f2e 7079 2c20 6578 616d 706c 655f  t__.py, example_
+000006d0: 6461 7461 2c20 696d 6167 6573 2c20 6e61  data, images, na
+000006e0: 7061 7269 5f63 6c75 7374 6572 735f 706c  pari_clusters_pl
+000006f0: 6f74 7465 722f 5f67 6574 5f63 6f6c 6f72  otter/_get_color
+00000700: 6d61 702e 7079 0d0a 6261 6e6e 6564 2d6d  map.py..banned-m
+00000710: 6f64 756c 6573 203d 2050 7951 7435 203d  odules = PyQt5 =
+00000720: 2075 7365 2071 7470 790d 0a09 5079 5369   use qtpy...PySi
+00000730: 6465 3220 3d20 7573 6520 7174 7079 0d0a  de2 = use qtpy..
+00000740: 0d0a 5b69 736f 7274 5d0d 0a70 726f 6669  ..[isort]..profi
+00000750: 6c65 203d 2062 6c61 636b 0d0a 0d0a 5b65  le = black....[e
+00000760: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000770: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000780: 203d 2030 0d0a 0d0a                       = 0....
```


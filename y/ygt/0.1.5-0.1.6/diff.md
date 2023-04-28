# Comparing `tmp/ygt-0.1.5.tar.gz` & `tmp/ygt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.1.5.tar", last modified: Wed Apr 26 01:18:16 2023, max compression
+gzip compressed data, was "ygt-0.1.6.tar", last modified: Fri Apr 28 22:29:48 2023, max compression
```

## Comparing `ygt-0.1.5.tar` & `ygt-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.311863 ygt-0.1.5/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.5/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.5/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-26 01:18:16.311750 ygt-0.1.5/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     2443 2023-04-19 18:25:54.000000 ygt-0.1.5/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-26 01:05:06.000000 ygt-0.1.5/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-26 01:18:16.311896 ygt-0.1.5/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.5/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.296095 ygt-0.1.5/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.303400 ygt-0.1.5/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.5/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.5/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.5/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5234 2023-04-25 12:51:05.000000 ygt-0.1.5/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.304277 ygt-0.1.5/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.5/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    12952 2023-04-26 00:07:28.000000 ygt-0.1.5/src/ygt/freetypeFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.311475 ygt-0.1.5/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.5/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.5/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.5/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.5/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.5/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.5/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.5/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.5/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.5/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.5/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    56264 2023-04-21 04:37:29.000000 ygt-0.1.5/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    65307 2023-04-25 21:18:30.000000 ygt-0.1.5/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.5/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   116392 2023-04-25 21:18:08.000000 ygt-0.1.5/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   137596 2023-04-24 10:33:58.000000 ygt-0.1.5/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.5/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    22140 2023-04-26 00:03:21.000000 ygt-0.1.5/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10040 2023-04-21 04:31:07.000000 ygt-0.1.5/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5674 2023-04-22 03:26:07.000000 ygt-0.1.5/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.5/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-26 01:18:16.304167 ygt-0.1.5/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     2839 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-26 01:18:16.000000 ygt-0.1.5/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.5/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.421758 ygt-0.1.6/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.6/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.6/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3734 2023-04-28 22:29:48.421633 ygt-0.1.6/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3338 2023-04-28 20:30:43.000000 ygt-0.1.6/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-28 22:27:57.000000 ygt-0.1.6/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-28 22:29:48.421793 ygt-0.1.6/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.6/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.406686 ygt-0.1.6/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.413190 ygt-0.1.6/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.6/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.6/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.6/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5234 2023-04-25 12:51:05.000000 ygt-0.1.6/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.414149 ygt-0.1.6/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.6/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12952 2023-04-26 00:07:28.000000 ygt-0.1.6/src/ygt/freetypeFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.421360 ygt-0.1.6/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.6/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.6/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.6/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.6/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.6/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.6/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.6/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.6/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.6/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.6/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    56264 2023-04-21 04:37:29.000000 ygt-0.1.6/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    65557 2023-04-28 10:05:58.000000 ygt-0.1.6/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.6/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   121428 2023-04-28 11:52:09.000000 ygt-0.1.6/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   141294 2023-04-28 12:16:44.000000 ygt-0.1.6/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.6/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22566 2023-04-28 18:49:42.000000 ygt-0.1.6/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10040 2023-04-21 04:31:07.000000 ygt-0.1.6/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5674 2023-04-22 03:26:07.000000 ygt-0.1.6/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.6/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-28 22:29:48.414038 ygt-0.1.6/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3734 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-28 22:29:48.000000 ygt-0.1.6/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.6/src/ygt.py
```

### Comparing `ygt-0.1.5/LICENSE` & `ygt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/PKG-INFO` & `ygt-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: ygt
-Version: 0.1.5
-Summary: A graphical hint editor for TrueType fonts
-Author-email: "Peter S. Baker" <b.tarde@mail.com>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ygt
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
 - it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
@@ -26,23 +14,41 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-### Version 0.1.24 (2023-4-19)
+### Version 0.1.6 (2023-4-28)
+
+Select more than one untouched point when adding shift, align, or interpolate hints to create a hint with a set as target. This formerly had to be done with a separate “Make Set” command.
+
+“Make Set” command has been removed as unnecessary.
+
+To add a point to a shift, align, or interpolate hint, select the hint and at least one untouched point, and press the **plus** key.
+
+To delete a point or points from a shift, align, or interpolate hint, select one ore more points belonging to the hint and press the **hyphen** or **minus** key.
+
+Corrected background color of preview panels when dark theme is active.
+
+### Version 0.1.5 (2023-4-25)
+
+Various UI refinements: initial scaling of glyphs, spacebar to temporarily switch to panning mode, and more.
+
+User now confronts only one kind of stem hint: Ygt guesses (more or less accurately) the distance type.
+
+### Version 0.1.4 (2023-4-19)
 
 When we read a UFO, we do not rename glyphs. This prevents incompatibilities between in-memory font and font on disk, and it simplifies export. However, it may complicate shifting back and forth between UFO and YAML modes.
 
 Ygt sometimes hung when summoning a Font View window for fonts read from UFO. This is now fixed.
 
 Program now (partly) honors dark themes on various platforms.
 
-### Version 0.1.23 (2023-4-17)
+### Version 0.1.3 (2023-4-17)
 
 changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
 ```
 s/blackspace/blackdist/g
 s/whitesapce/whitedist/g
 s/grayspace/graydist/g
 ```
```

### Comparing `ygt-0.1.5/src/ygt/autohint_trash.py` & `ygt-0.1.6/src/ygt/autohint_trash.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/cvGuesser.py` & `ygt-0.1.6/src/ygt/cvGuesser.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/fontViewDialog.py` & `ygt-0.1.6/src/ygt/fontViewDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.1.6/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/freetypeFont.py` & `ygt-0.1.6/src/ygt/freetypeFont.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/align.png` & `ygt-0.1.6/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/anchor.png` & `ygt-0.1.6/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/black_distance.png` & `ygt-0.1.6/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/cursor-icon-off.png` & `ygt-0.1.6/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/cursor-icon-on.png` & `ygt-0.1.6/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/cv.png` & `ygt-0.1.6/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/cv_guess.png` & `ygt-0.1.6/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/gray_distance.png` & `ygt-0.1.6/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/hand-icon-off.png` & `ygt-0.1.6/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/hand-icon-on.png` & `ygt-0.1.6/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/horizontal-off.png` & `ygt-0.1.6/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/horizontal-on.png` & `ygt-0.1.6/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/interpolate.png` & `ygt-0.1.6/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/make_set.png` & `ygt-0.1.6/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/program.png` & `ygt-0.1.6/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/shift.png` & `ygt-0.1.6/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/stem_distance.png` & `ygt-0.1.6/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/vertical-off.png` & `ygt-0.1.6/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/vertical-on.png` & `ygt-0.1.6/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/icons/white_distance.png` & `ygt-0.1.6/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/macfuncDialog.py` & `ygt-0.1.6/src/ygt/macfuncDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/makeCVDialog.py` & `ygt-0.1.6/src/ygt/makeCVDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/window.py` & `ygt-0.1.6/src/ygt/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,18 +538,18 @@
                 QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_A), # type: ignore
                 QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
                 QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
             ]
         )
         self.anchor_action.setEnabled(False)
 
-        self.make_set_action = self.toolbar.addAction("Make Set (K)")
-        self.make_set_action.setIcon(QIcon(QPixmap(self.icon_path + "make_set.png")))
-        self.make_set_action.setShortcut(QKeySequence(Qt.Key.Key_K))
-        self.make_set_action.setEnabled(False)
+        #self.make_set_action = self.toolbar.addAction("Make Set (K)")
+        #self.make_set_action.setIcon(QIcon(QPixmap(self.icon_path + "make_set.png")))
+        #self.make_set_action.setShortcut(QKeySequence(Qt.Key.Key_K))
+        #self.make_set_action.setEnabled(False)
 
         self.make_cv_guess_action = self.toolbar.addAction("Guess Control Value (?)")
         self.make_cv_guess_action.setIcon(
             QIcon(QPixmap(self.icon_path + "cv_guess.png"))
         )
         self.make_cv_guess_action.setShortcut(QKeySequence(Qt.Key.Key_Question))
         self.make_cv_guess_action.setEnabled(False)
@@ -609,17 +609,20 @@
         if self.current_axis == "y":
             self.vertical_action.setChecked(True)
         else:
             self.horizontal_action.setChecked(True)
 
     @pyqtSlot(object)
     def preview_ready(self, args: dict) -> None:
-        glyph_index = args["gindex"][self.preview_glyph_name]
-        self.yg_preview.fetch_glyph(args["font"], glyph_index)
-        self.yg_preview.update()
+        try:
+            glyph_index = args["gindex"][self.preview_glyph_name]
+            self.yg_preview.fetch_glyph(args["font"], glyph_index)
+            self.yg_preview.update()
+        except Exception:
+            pass
 
     @pyqtSlot()
     def toggle_auto_preview(self) -> None:
         self.auto_preview_update = not self.auto_preview_update
         try:
             self.glyph_pane.viewer.yg_glyph.set_auto_preview_connection()
         except Exception as e:
@@ -830,15 +833,15 @@
         self.stem_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.anchor_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.interpolate_action.triggered.connect(
             self.glyph_pane.make_hint_from_selection
         )
         self.shift_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.align_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
-        self.make_set_action.triggered.connect(self.glyph_pane.make_set)
+        # self.make_set_action.triggered.connect(self.glyph_pane.make_set)
         self.make_cv_action.triggered.connect(self.glyph_pane.make_control_value)
         self.make_cv_guess_action.triggered.connect(self.glyph_pane.guess_cv)
         self.vertical_action.toggled.connect(self.glyph_pane.switch_to_y)
         self.horizontal_action.toggled.connect(self.glyph_pane.switch_to_x)
 
     def setup_edit_connections(self) -> None:
         self.edit_cvt_action.triggered.connect(self.edit_cvt)
@@ -1340,48 +1343,51 @@
         if selection_profile[0] == 0 and selection_profile[1] == 1:
             # enable anchor button
             self.anchor_action.setEnabled(True)
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
-            self.make_set_action.setEnabled(False)
+            # self.make_set_action.setEnabled(False)
         elif selection_profile[0] == 1 and selection_profile[1] >= 1:
             # Enable make set button
-            if 1 in selection_profile[2] or 2 in selection_profile[2]:
-                self.make_set_action.setEnabled(True)
-            else:
-                self.make_set_action.setEnabled(False)
+            #if 1 in selection_profile[2] or 2 in selection_profile[2]:
+            #    self.make_set_action.setEnabled(True)
+            #else:
+            #    self.make_set_action.setEnabled(False)
+            # stem_action only if 1 pt touched and 1 pt untouched.
             if selection_profile[1] == 1:
-                # Enable link buttons
                 self.stem_action.setEnabled(True)
+            else:
+                self.stem_action.setEnabled(False)
+            # shift_action and align_action if 1 pt touched and 1 or more untouched.
+            if selection_profile[1] >= 1:
                 self.shift_action.setEnabled(True)
                 self.align_action.setEnabled(True)
             else:
-                self.stem_action.setEnabled(False)
                 self.shift_action.setEnabled(False)
                 self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
-        elif selection_profile[0] == 2 and selection_profile[1] == 1:
+        elif selection_profile[0] == 2 and selection_profile[1] >= 1:
             # Enable interpolation button
             self.interpolate_action.setEnabled(True)
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
-            self.make_set_action.setEnabled(False)
+            #self.make_set_action.setEnabled(False)
         else:
             # "Disable all hint editing buttons
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
-            self.make_set_action.setEnabled(False)
+            #self.make_set_action.setEnabled(False)
 
     @pyqtSlot()
     def clean_changed(self):
         self.set_window_title()
 
     def set_window_title(self) -> None:
         """And also the status bar"""
@@ -1677,15 +1683,15 @@
             if self.top_window.isActiveWindow():
                 self.top_window.preferences["top_window"] = self.top_window
         return super().eventFilter(source, event)
 
 
 def main():
     # from PyQt6.QtGui import QPalette
-    # print(dir(QPalette))
+    # print(dir(Qt))
     # print(inspect.getargspec(freetype.Face.get_glyph_name))
 
     app = QApplication([])
     font_id = QFontDatabase.addApplicationFont(os.path.dirname(__file__) + "/fonts/SourceCodePro-Regular.ttf")
     if font_id == -1:
         print("Can't find the font Source Code Pro.")
     top_window = MainWindow(app)
```

### Comparing `ygt-0.1.5/src/ygt/ygError.py` & `ygt-0.1.6/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/ygHintEditor.py` & `ygt-0.1.6/src/ygt/ygHintEditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,41 +57,56 @@
     QDialog,
     QInputDialog,
     QLineEdit,
     QGraphicsProxyWidget,
     QStyleOptionGraphicsItem,
 )
 from fontTools.pens.basePen import BasePen  # type: ignore
-from fontTools.pens.boundsPen import BoundsPen
+# from fontTools.pens.boundsPen import BoundsPen
 from .ygPreferences import ygPreferences
 
 
 HINT_ARROW_WIDTH = 3
 HINT_ANCHOR_WIDTH = 3
 HINT_LINK_WIDTH = 1
 HINT_ARROWHEAD_WIDTH = 2
-HINT_COLLECTION_COLOR = QColor(0, 255, 0, 128)
-HINT_COLLECTION_SELECT_COLOR = QColor(0, 205, 0, 128)
+
 HINT_ANCHOR_COLOR = QColor(255, 0, 255, 128)
+HINT_ANCHOR_DARK = QColor(255, 0, 255, 192)
 HINT_ANCHOR_SELECT_COLOR = QColor(175, 0, 175, 128)
+HINT_ANCHOR_SELECT_DARK = QColor(192, 0, 192, 192)
+
 HINT_STEM_COLOR = QColor(255, 0, 0, 128)
+HINT_STEM_DARK = QColor(255, 128, 176, 192)
 HINT_STEM_SELECT_COLOR = QColor(175, 0, 0, 128)
+HINT_STEM_SELECT_DARK = QColor(191, 0, 74, 192)
+
 HINT_SHIFT_COLOR = QColor(100, 100, 255, 128)
+HINT_SHIFT_DARK = QColor(96, 159, 191, 192)
 HINT_SHIFT_SELECT_COLOR = QColor(0, 0, 150, 128)
+HINT_SHIFT_SELECT_DARK = QColor(51, 186, 255, 192)
+
 HINT_ALIGN_COLOR = QColor(0, 255, 0, 128)
+HINT_ALIGN_DARK = QColor(191, 255, 209, 192)
 HINT_ALIGN_SELECT_COLOR = QColor(0, 205, 0, 128)
-HINT_LINK_COLOR = QColor(127, 127, 255, 255)
-HINT_LINK_SELECT_COLOR = QColor(87, 87, 215, 255)
+HINT_ALIGN_SELECT_DARK = QColor(96, 191, 122, 192)
+
 HINT_FUNC_COLOR = QColor(0, 205, 0, 128)
+HINT_FUNC_DARK = QColor(173, 204, 181, 192)
 HINT_FUNC_SELECT_COLOR = QColor(0, 105, 0, 128)
+HINT_FUNC_SELECT_DARK = QColor(38, 191, 74, 192)
+
 HINT_INTERPOLATE_COLOR = QColor(255, 127, 0, 128)
+HINT_INTERPOLATE_DARK = QColor(212, 187, 106, 192)
 HINT_INTERPOLATE_SELECT_COLOR = QColor(215, 87, 0, 128)
-SET_COLOR = QColor(128, 128, 128, 128)
-SET_SELECT_COLOR = QColor(128, 128, 128, 225)
-POINT_OFFCURVE_SELECTED = QColor(127, 127, 255, 255)
+HINT_INTERPOLATE_SELECT_DARK = QColor(255, 195, 0, 192)
+
+#SET_COLOR = QColor(128, 128, 128, 128)
+#SET_SELECT_COLOR = QColor(128, 128, 128, 225)
+
 POINT_ONCURVE_OUTLINE = QColor("red")
 POINT_OFFCURVE_FILL = QColor("white")
 POINT_ONCURVE_FILL = QColor("white")
 POINT_OFFCURVE_OUTLINE = QColor(127, 127, 255, 255)
 POINT_OFFCURVE_SELECTED = QColor(127, 127, 255, 255)
 POINT_ONCURVE_SELECTED = QColor(127, 127, 255, 255)
 PREVIEW_BASE_COLOR = QColor(64, 33, 31, 255)
@@ -100,42 +115,76 @@
 CHAR_OUTLINE_WIDTH = 1
 FUNC_BORDER_WIDTH = 2
 GLYPH_WIDGET_MARGIN = 50
 POINT_ONCURVE_DIA = 8
 POINT_OFFCURVE_DIA = 6
 HINT_BUTTON_DIA = 6
 
-HINT_COLOR = {
+HINT_COLOR = {}
+
+_HINT_COLOR = {
     "anchor": HINT_ANCHOR_COLOR,
     "align": HINT_ALIGN_COLOR,
     "shift": HINT_SHIFT_COLOR,
     "interpolate": HINT_INTERPOLATE_COLOR,
     "stem": HINT_STEM_COLOR,
     "whitedist": HINT_STEM_COLOR,
     "blackdist": HINT_STEM_COLOR,
     "graydist": HINT_STEM_COLOR,
     "move": HINT_STEM_COLOR,
     "macro": HINT_FUNC_COLOR,
     "function": HINT_FUNC_COLOR,
-    "set": SET_COLOR,
+    # "set": SET_COLOR,
+}
+
+_HINT_DARK = {
+    "anchor": HINT_ANCHOR_DARK,
+    "align": HINT_ALIGN_DARK,
+    "shift": HINT_SHIFT_DARK,
+    "interpolate": HINT_INTERPOLATE_DARK,
+    "stem": HINT_STEM_DARK,
+    "whitedist": HINT_STEM_DARK,
+    "blackdist": HINT_STEM_DARK,
+    "graydist": HINT_STEM_DARK,
+    "move": HINT_STEM_DARK,
+    "macro": HINT_FUNC_DARK,
+    "function": HINT_FUNC_DARK,
+    # "set": SET_COLOR,
 }
 
-SELECTED_HINT_COLOR = {
+SELECTED_HINT_COLOR = {}
+
+_SELECTED_HINT_COLOR = {
     "anchor": HINT_ANCHOR_SELECT_COLOR,
     "align": HINT_ALIGN_SELECT_COLOR,
     "shift": HINT_SHIFT_SELECT_COLOR,
     "interpolate": HINT_INTERPOLATE_SELECT_COLOR,
     "stem": HINT_STEM_SELECT_COLOR,
     "whitedist": HINT_STEM_SELECT_COLOR,
     "blackdist": HINT_STEM_SELECT_COLOR,
     "graydist": HINT_STEM_SELECT_COLOR,
     "move": HINT_STEM_SELECT_COLOR,
     "macro": HINT_FUNC_SELECT_COLOR,
     "function": HINT_FUNC_SELECT_COLOR,
-    "set": SET_SELECT_COLOR,
+    # "set": SET_SELECT_COLOR,
+}
+
+_SELECTED_HINT_DARK = {
+    "anchor": HINT_ANCHOR_SELECT_DARK,
+    "align": HINT_ALIGN_SELECT_DARK,
+    "shift": HINT_SHIFT_SELECT_DARK,
+    "interpolate": HINT_INTERPOLATE_SELECT_DARK,
+    "stem": HINT_STEM_SELECT_DARK,
+    "whitedist": HINT_STEM_SELECT_DARK,
+    "blackdist": HINT_STEM_SELECT_DARK,
+    "graydist": HINT_STEM_SELECT_DARK,
+    "move": HINT_STEM_SELECT_DARK,
+    "macro": HINT_FUNC_SELECT_DARK,
+    "function": HINT_FUNC_SELECT_DARK,
+    # "set": SET_SELECT_COLOR,
 }
 
 # Classes in this file:
 
 # QtPen (BasePen): copied from fontTools so we could drop a reference to Qt5.
 # ygSelectable: inherited by objects that can be selected.
 # ygHintView(QGraphicsItem, ygSelectable): Interface with a hint (ygModel.ygHint)
@@ -325,15 +374,15 @@
 
     def contains(self, pt: QPointF) -> bool:
         if len(self.graphical_hint) >= 1:
             for g in self.graphical_hint:
                 if g.contains(pt):
                     return True
         return False
-
+    
     def mouse_over_point(self, pt: QPointF) -> "ygPointMarker":
         """In ygHintView. Returns a ygPointMarker."""
         if len(self.graphical_hint) >= 1:
             for g in self.graphical_hint:
                 if type(g) is ygPointMarker and g.contains(pt):
                     return g
         return None
@@ -1359,14 +1408,16 @@
     sig_name_points = pyqtSignal(object)
 
     def __init__(
             self, preferences: ygPreferences,
             yg_glyph: ygGlyph,
             owner: Optional["ygGlyphView"] = None) -> None:
         """yg_glyph is a ygGlyph object from ygModel."""
+        global HINT_COLOR, SELECTED_HINT_COLOR, POINT_OFFCURVE_FILL, POINT_ONCURVE_FILL, POINT_OFFCURVE_SELECTED, POINT_ONCURVE_SELECTED
+
         self.preferences = preferences
 
         # Set up glyph info
 
         self.yg_glyph = yg_glyph
         self.owner = owner
 
@@ -1376,14 +1427,29 @@
         # self.yg_hint_view_index: dict = {}
         self.yg_hint_view_list: list = []
         super(ygGlyphScene, self).__init__()
         self.cv_error_msg = "Error while looking for a control value."
 
         # Current display preferences
 
+        # Auto-detect if we have dark mode. We need to know so we can set
+        # hint colors (not controlled by the system) to appropriate values.
+        text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
+        bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+        self.dark_theme = text_hsv_value > bg_hsv_value
+        if self.dark_theme:
+            HINT_COLOR = _HINT_DARK
+            SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
+            POINT_OFFCURVE_FILL = QColor("black")
+            POINT_ONCURVE_FILL = QColor("black")
+            POINT_OFFCURVE_SELECTED = QColor(QColor(137, 207, 240))
+            POINT_ONCURVE_SELECTED = QColor(QColor(137, 207, 240))
+        else:
+            HINT_COLOR = _HINT_COLOR
+            SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
         if self.preferences.top_window().show_off_curve_points != None:
             self.off_curve_points_showing = self.preferences.top_window().show_off_curve_points
         else:
             self.off_curve_points_showing = self.preferences.show_off_curve_points()
         self.point_numbers_showing = self.preferences.top_window().show_point_numbers
         self.zoom_factor = 1.0
         self.initial_zoom_factor = None
@@ -1594,14 +1660,17 @@
     #
 
     def drawBackground(self, painter: QPainter, rect) -> None:
         """The glyph outline is drawn as the background layer for this scene.
         Points and hints are drawn in the item layer, and the foreground
         layer is not used at this time.
         """
+
+        global HINT_COLOR, SELECTED_HINT_COLOR
+
         if not self.initial_zoom_factor:
             visible_x = rect.width()
             visible_y = rect.height()
             optimal_x = round(visible_x * 0.8)
             optimal_y = round(visible_y * 0.8)
             width, height = self.yg_glyph.dimensions()
             if width != 0:
@@ -1622,22 +1691,23 @@
 
         painter.scale(1.0, -1.0)
         painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
 
         pen = painter.pen()
 
         if self.preferences["show_metrics"]:
-            text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
-            bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
-            dark_theme = text_hsv_value > bg_hsv_value
             pen.setWidth(1)
-            if dark_theme:
+            if self.dark_theme:
                 pen.setColor(QColor(200, 200, 200, 50))
+                HINT_COLOR = _HINT_DARK
+                SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
             else:
                 pen.setColor(QColor(50, 50, 50, 50))
+                HINT_COLOR = _HINT_COLOR
+                SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
             painter.setPen(pen)
             painter.drawLine(QLine(-abs(self.xTranslate), 0, round(self.width()), 0))
             ya = -abs(self.yTranslate)
             painter.drawLine(QLine(0, ya, 0, round(self.height())))
             painter.drawLine(QLine(self.adv, ya, self.adv, round(self.height())))
 
         pen.setWidth(CHAR_OUTLINE_WIDTH)
@@ -1725,45 +1795,44 @@
                     if self.point_numbers_showing:
                         p.add_label()
                 else:
                     p.hide()
                     if self.point_numbers_showing:
                         p.del_label()
 
-    def make_set(self) -> None:
-        """In the hint model, the target can be either a ygPoint or a ygSet.
-        This function takes the current selection, several ygPoint, and turns
-        them into a ygSet, which it substitutes for the ygPoint. Note that
-        exactly one selected point must be touched, and at least one
-        selected point must be untouched.
-
-        """
-        selected_points = self.selected_objects(True)
-        touched_points = []
-        untouched_points = []
-        for s in selected_points:
-            if s.touched:
-                touched_points.append(s)
-            else:
-                untouched_points.append(s)
-        if len(untouched_points) < 1 or len(touched_points) != 1:
-            return
-        touched_point = touched_points[0]
-        hint = touched_point.owners[0]
-        hint_model = hint.yg_hint
-        if not hint_model.hint_type() in ["shift", "align", "interpolate"]:
-            return
-        new_list = []
-        for p in selected_points:
-            new_list.append(self._model_point(p))
-        # params: ygModel.ygHint, list of ygModel.ygPoint, touched ygModel.ygPoint, callback func.
-        self.yg_glyph.make_set(
-            hint_model, new_list, touched_point.yg_point, hint._update_touches
-        )
-        self.yg_glyph.hint_changed(hint_model)
+    #def make_set(self) -> None:
+    #    """In the hint model, the target can be either a ygPoint or a ygSet.
+    #    This function takes the current selection, several ygPoint, and turns
+    #    them into a ygSet, which it substitutes for the ygPoint. Note that
+    #    exactly one selected point must be touched, and at least one
+    #    selected point must be untouched.
+    #    """
+    #    selected_points = self.selected_objects(True)
+    #    touched_points = []
+    #    untouched_points = []
+    #    for s in selected_points:
+    #        if s.touched:
+    #            touched_points.append(s)
+    #        else:
+    #            untouched_points.append(s)
+    #    if len(untouched_points) < 1 or len(touched_points) != 1:
+    #        return
+    #    touched_point = touched_points[0]
+    #    hint = touched_point.owners[0]
+    #    hint_model = hint.yg_hint
+    #    if not hint_model.hint_type() in ["shift", "align", "interpolate"]:
+    #        return
+    #    new_list = []
+    #    for p in selected_points:
+    #        new_list.append(self._model_point(p))
+    #    # params: ygModel.ygHint, list of ygModel.ygPoint, touched ygModel.ygPoint, callback func.
+    #    self.yg_glyph.make_set(
+    #        hint_model, new_list, touched_point.yg_point, hint._update_touches
+    #    )
+    #    self.yg_glyph.hint_changed(hint_model)
 
     def make_control_value(self) -> None:
         """ With one or two points selected, launch a dialog for making a pos or dist CV.
         """
         sel = self.selected_objects(True)
         if len(sel) == 0:
             return
@@ -1913,14 +1982,71 @@
         for o in oo:
             if type(o) is ygHintView:
                 hh.append(o.yg_hint)
         if len(hh) > 0:
             # Call a function in the model.
             hh[0].delete_hints(hh)
 
+    def add_to_set(self):
+        """Do validity check on current selection, then call ygHint.add_points."""
+        profile = self.selection_profile()
+        # At least one non-touched point selected
+        # Exactly one hint selected
+        # hint type is shift, align, or interpolate [1, 2]
+        # exactly one hint selected
+        if (profile[0] == 0
+            and profile[1] > 0
+            and profile[3][0] in [1, 2]
+            and profile[4] == 1
+        ):
+            objects = self.selected_objects(False)
+            hints = []
+            points = []
+            for o in objects:
+                if type(o) is ygPointView:
+                    points.append(self._model_point(o))
+                if type(o) is ygHintView:
+                    hints.append(self._model_hint(o))
+            hints[0].add_points(points)
+
+    def delete_from_set(self):
+        profile = self.selection_profile()
+        # if no selected points are touched,
+        # or there are untouched points selected,
+        # or there is not exactly one owner (hint) type,
+        # or the one type is not shift, align, or interpolate,
+        # or any hints are selected,
+        # then we do nothing.
+        if (
+            profile[0] == 0
+            or profile[1] > 0
+            or len(profile[2]) != 1
+            or not profile[2][0] in [1, 2]
+            or len(profile[3]) != 0
+        ):
+            return
+        selected_points = self.selected_objects(True)
+        if len(selected_points) > 0:
+            try:
+                owner_hint = None
+                hint_list = self.yg_glyph.hints()
+                model_points = []
+                for p in selected_points:
+                    model_points.append(self._model_point(p))
+                for h in hint_list:
+                    if h.contains_points(model_points):
+                        owner_hint = h
+                        break
+                if not owner_hint:
+                    print("Couldn't get an owner hint")
+                    return
+                owner_hint.delete_points(model_points)
+            except Exception as e:
+                pass
+
     #
     # Utilities
     #
 
     def get_scene(self) -> "ygGlyphScene":
         """Returns the current scene (always this object!)
 
@@ -1988,35 +2114,43 @@
 
     def selection_profile(self) -> Tuple[int, int, List[int], List[int]]:
         """Surveys the current selection and returns a tuple containing:
         - The number of touched points
         - The number of untouched points
         - The (integer) types of the owners of touched points
         - The (integer) types of any selected hints
+        - The number of selected hints
         """
         s = self.selected_objects(True)
         touched_point_count = untouched_point_count = 0
         owner_types = []
         for ss in s:
             if ss.touched:
                 touched_point_count += 1
                 for h in ss.owners:
-                    owner_types.append(hint_type_nums[h.yg_hint.hint_type()])
+                    htn = hint_type_nums[h.yg_hint.hint_type()]
+                    if not htn in owner_types:
+                        owner_types.append(htn)
             else:
                 untouched_point_count += 1
         selected_hint_types = []
         s = self.selected_objects(False)
+        hint_count = 0
         for ss in s:
             if type(ss) is ygHintView:
-                selected_hint_types.append(hint_type_nums[ss.yg_hint.hint_type()])
+                hint_count += 1
+                htn = hint_type_nums[ss.yg_hint.hint_type()]
+                if not htn in selected_hint_types:
+                    selected_hint_types.append(htn)
         return (
             touched_point_count,
             untouched_point_count,
             owner_types,
             selected_hint_types,
+            hint_count,
         )
 
     def selected_objects(self, points_only: bool) -> list:
         """Get a list of objects (points and hints) selected by the user.
 
         Parameters:
         points_only (bool): if true, return only selected points (not hints)
@@ -2208,15 +2342,14 @@
                 self.addItem(yg_hint_view)
             else:
                 raise Exception(
                     "Something went wrong with gtarget in _make_visible_hint"
                 )
         else:
             raise Exception("Unknown hint type " + str(hint_type_num))
-        # self.yg_hint_view_index[hint.id] = yg_hint_view
         self.yg_hint_view_list.append(yg_hint_view)
         return yg_hint_view
 
     @pyqtSlot(dict)
     def make_macfunc(self, _params: dict) -> None:
         hint_type = _params["hint_type"]
         name = _params["name"]
@@ -2267,56 +2400,69 @@
                         hint_type = stemFinder(
                             self._model_point(pp[0]),
                             self._model_point(pp[1]),
                             self.yg_glyph,
                         ).get_color()
                 except Exception as e:
                     print(e)
-                # ref should be a touched point and target an untouched point.
-                # If it's the other way around, reverse them.
-                if pp[1].touched and not pp[0].touched:
-                    pp[0], pp[1] = pp[1], pp[0]
-                target_name = self._model_point(pp[1]).preferred_label()
-                ref_name = self._model_point(pp[0]).preferred_label()
-                h = {"ptid": target_name, "ref": ref_name, "rel": hint_type}
+                ref_name = ""
+                target_names = []
+                for ppp in pp:
+                    if ppp.touched:
+                        ref_name = self._model_point(ppp).preferred_label()
+                    else:
+                        target_names.append(str(self._model_point(ppp).preferred_label()))
+                if len(target_names) == 1 or hint_type_num == 3:
+                    tgt = target_names[0]
+                else:
+                    tgt = target_names
+                # This should not happen if we've filtered properly before calling this.
+                if not ref_name or len(target_names) == 0:
+                    return
+                h = {"ptid": tgt, "ref": ref_name, "rel": hint_type}
                 new_yg_hint = ygHint(self.yg_glyph, h)
                 dr = self.get_round_default(new_yg_hint)
                 if dr != None:
                     new_yg_hint.set_round(dr)
                 if ctrl and hint_type_num == 3:
                     self.guess_cv_for_hint(new_yg_hint)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
         if hint_type_num == 2:
             if pplen >= 3:
-                if pplen > 3:
-                    del pp[3:]
+                #if pplen > 3:
+                #    del pp[3:]
                 # If two of the three selected points are touched, they are the
                 # reference points, and the untouched point is the target.
                 # Otherwise, sort the points by x or y position: the middle one
                 # is the target, and the ones on the ends are reference points.
                 # If the program makes the wrong choice, user can rearrange
                 # things in the editor.
                 touched_points = []
                 untouched_points = []
                 for t in pp:
                     if type(t) is ygPointView:
                         if t.touched:
                             touched_points.append(self._model_point(t))
                         else:
                             untouched_points.append(self._model_point(t))
-                if len(touched_points) == 2 and len(untouched_points) == 1:
+                if len(touched_points) == 2 and len(untouched_points) >= 1:
                     touched_names = [
                         touched_points[0].preferred_label(),
                         touched_points[1].preferred_label(),
                     ]
-                    untouched_name = untouched_points[0].preferred_label()
+                    if len(untouched_points) == 1:
+                        tgt = untouched_points[0].preferred_label()
+                    else:
+                        tgt = []
+                        for p in untouched_points:
+                            tgt.append(p.preferred_label())
                     # Think about this more. Why does mypy not like it?
-                    h = {"ptid": untouched_name, "ref": touched_names, "rel": hint_type}  # type: ignore
+                    h = {"ptid": tgt, "ref": touched_names, "rel": hint_type}  # type: ignore
                     new_yg_hint = ygHint(self.yg_glyph, h)
                 else:
                     newlist = []
                     for p in pp:
                         newlist.append(self._model_point(p))
                     sorter = ygPointSorter(self.yg_glyph.current_axis())
                     sorter.sort(newlist)
@@ -2438,16 +2584,16 @@
             Set control value: Done
             Set distance type for stem hints: Done
             Reverse stem hint: Done
             Additional parameters for functions and macros: Done
             Rearrange function/macro point params: Done
             Add point to function call: Not yet started
             Convert target point to target set in function/macro: Not yet started
-            Set target and reference points for function/macro: Done
-            Make set: Doesn't yet work for functions/macros
+            Set target and reference points for function/macro: Done bug disabled
+            Make set: Doesn't yet work for functions/macros. Disabled as possibly not needed.
             Create function call: Done
             Create macro call: Done
 
         """
 
         cmenu = QMenu()
         selected_points = self.selected_objects(True)
@@ -2985,55 +3131,52 @@
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         self.viewer.make_hint_from_selection(
             menu_to_hint_type[self.sender().text()], ctrl=with_ctrl, shift=with_shift  # type: ignore
         )
 
-    @pyqtSlot()
-    def make_set(self) -> None:
-        self.viewer.make_set()
+    #@pyqtSlot()
+    #def make_set(self) -> None:
+    #    self.viewer.make_set()
 
     # Why does sender return None when we use the decorator? What's best in this
     # situation? Here are problems: sender_text param is not consulted. Should it be
     # omitted? Make sure params match, esp. if we change them.
     # @pyqtSlot(object)
     def zoom(self, sender_text: str) -> None:
         sender_text = self.sender().text()  # type: ignore
         if sender_text == "Original Size":
-            #self.viewer.set_zoom_factor(1)
             self.viewer.set_zoom_factor(self.viewer.initial_zoom_factor)
         elif sender_text == "Zoom In":
             if self.viewer.zoom_factor <= 5.75:
                 self.viewer.set_zoom_factor(self.viewer.zoom_factor + 0.25)
         elif sender_text == "Zoom Out":
             if self.viewer.zoom_factor >= 0.5:
                 self.viewer.set_zoom_factor(self.viewer.zoom_factor - 0.25)
-
-        # What I'd *like* to do here is keep the center of the viewport centered
-        # after the zoom. But I haven't been able to make this work with the
-        # Qt methods I've tried. So we're defaulting to having the center of the
-        # glyph in the center--which at least is easy.
-
-        # v = self.viewport().geometry()
-        # qp = QPoint(round(v.x() + (v.width() / 2)), round(v.y() + (v.height() / 2)))
-        # self.centerOn(self.mapToScene(qp))
-
-        # self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
         self.centerOn(self.viewer.center_x, self.viewer.mid_point_y())
 
     def keyPressEvent(self, event) -> None:
+        # 1. Delete key will delete any selected hints.
+        # 2. Spacebar will shift Qt drag mode to ScrollHandDrag while it is
+        #    down. For panning the screen.
         if event.key() in [16777219, 16777223]:
             self.viewer.delete_selected_hints()
+        elif event.key() == Qt.Key.Key_Plus:
+            self.viewer.add_to_set()
+        elif event.key() == Qt.Key.Key_Minus:
+            self.viewer.delete_from_set()
         elif event.key() == 32 and not event.isAutoRepeat():
             self.drag_mode_backup = self.dragMode()
             if self.drag_mode_backup == QGraphicsView.DragMode.NoDrag:
                 self.sig_toggle_drag_mode.emit(QGraphicsView.DragMode.ScrollHandDrag)
 
     def keyReleaseEvent(self, event):
+        # Releasting spacebar shifts Qt drag mode back to whatever it was before
+        # spacebar was pressed.
         if event.key() == 32 and not event.isAutoRepeat():
             if self.drag_mode_backup != self.dragMode():
                 self.sig_toggle_drag_mode.emit(self.drag_mode_backup)
 
 
     def focusInEvent(self, event) -> None:
         self.viewer.yg_glyph.undo_stack.setActive(True)
```

### Comparing `ygt-0.1.5/src/ygt/ygModel.py` & `ygt-0.1.6/src/ygt/ygModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 # setMacFuncOtherArgsCommand(glyphEditCommand): Glyph editing command.
 # swapMacFuncPointsCommand(glyphEditCommand): Glyph editing command.
 # cleanupGlyphCommand(glyphEditCommand): Glyph editing command.
 # changeDistanceTypeCommand(glyphEditCommand): Glyph editing command.
 # toggleMinDistCommand(glyphEditCommand): Glyph editing command.
 # changeCVCommand(glyphEditCommand): Glyph editing command.
 # toggleRoundingCommand(glyphEditCommand): Glyph editing command.
-# makeSetCommand(glyphEditCommand): Glyph editing command.
+# makeSetCommand(glyphEditCommand): Glyph editing command. (disabled -- perhaps not needed)
 # addHintCommand(glyphEditCommand): Glyph editing command.
 # deleteHintsCommand(glyphEditCommand): Glyph editing command.
 # reverseHintCommand(glyphEditCommand): Glyph editing command.
 # switchAxisCommand(QUndoCommand): Glyph editing command.
 # glyphAddPropertyCommand(QUndoCommand): Glyph editing command.
 # glyphDeletePropertyCommand(QUndoCommand): Glyph editing command.
 #
@@ -1810,43 +1810,43 @@
             else:
                 self.hint._source["round"] = current_round
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "toggleRoundingCommand").test()
         self.send_signal()
 
 
-class makeSetCommand(glyphEditCommand):
-    def __init__(
-        self,
-        glyph: "ygGlyph",
-        hint: "ygHint",
-        pt_list: list,
-        touched_point: Optional[ygPoint],
-        callback: Callable,
-    ) -> None:
-        super().__init__(glyph)
-        self.hint = hint
-        self.pt_list = pt_list
-        self.touched_point = touched_point
-        self.callback = callback
-        self.setText("Make Set")
-
-    def redo(self) -> None:
-        if self.redo_state:
-            self.redo_state.restore()
-        else:
-            sorter = ygPointSorter(self.yg_glyph.current_axis())
-            sorter.sort(self.pt_list)
-            set = ygSet(self.pt_list)
-            set._main_point = self.touched_point
-            self.hint.set_target(set.id_list())
-            self.callback()
-            self.redo_state = glyphSaver(self.yg_glyph)
-        glyphSourceTester(self.yg_glyph, "makeSetCommand").test()
-        self.send_signal()
+#class makeSetCommand(glyphEditCommand):
+#    def __init__(
+#        self,
+#        glyph: "ygGlyph",
+#        hint: "ygHint",
+#        pt_list: list,
+#        touched_point: Optional[ygPoint],
+#        callback: Callable,
+#    ) -> None:
+#        super().__init__(glyph)
+#        self.hint = hint
+#        self.pt_list = pt_list
+#        self.touched_point = touched_point
+#        self.callback = callback
+#        self.setText("Make Set")
+#
+#    def redo(self) -> None:
+#        if self.redo_state:
+#            self.redo_state.restore()
+#        else:
+#            sorter = ygPointSorter(self.yg_glyph.current_axis())
+#            sorter.sort(self.pt_list)
+#            set = ygSet(self.pt_list)
+#            set._main_point = self.touched_point
+#            self.hint.set_target(set.id_list())
+#            self.callback()
+#            self.redo_state = glyphSaver(self.yg_glyph)
+#        glyphSourceTester(self.yg_glyph, "makeSetCommand").test()
+#        self.send_signal()
 
 
 class addHintCommand(glyphEditCommand):
     def __init__(
         self, glyph: "ygGlyph", hint: "ygHint", conditional: bool = False
     ) -> None:
         super().__init__(glyph)
@@ -1914,14 +1914,48 @@
             )
             self.yg_glyph._rebuild_current_block()
             self.redo_state = glyphSaver(self.yg_glyph)
         glyphSourceTester(self.yg_glyph, "reverseHintCommand").test()
         self.send_signal()
 
 
+class addPointsCommand(glyphEditCommand):
+    def __init__(self, glyph: "ygGlyph", hint: "ygHint", p_list: list) -> None:
+        super().__init__(glyph)
+        self.hint = hint
+        self.p_list = p_list
+        self.setText("Adds points to hint")
+
+    def redo(self) -> None:
+        if self.redo_state:
+            self.redo_state.restore()
+        else:
+            self.hint._add_points(self.p_list)
+            self.redo_state = glyphSaver(self.yg_glyph)
+        glyphSourceTester(self.yg_glyph, "addPointsCommand").test()
+        self.send_signal()
+
+
+class deletePointsCommand(glyphEditCommand):
+    def __init__(self, glyph: "ygGlyph", hint: "ygHint", p_list: list) -> None:
+        super().__init__(glyph)
+        self.hint = hint
+        self.p_list = p_list
+        self.setText("Delete points from hint")
+
+    def redo(self) -> None:
+        if self.redo_state:
+            self.redo_state.restore()
+        else:
+            self.hint._delete_points(self.p_list)
+            self.redo_state = glyphSaver(self.yg_glyph)
+        glyphSourceTester(self.yg_glyph, "deletePointsCommand").test()
+        self.send_signal()
+
+
 class switchAxisCommand(QUndoCommand):
     def __init__(self, g: "ygGlyph", prefs: ygPreferences, new_axis: str) -> None:
         super().__init__()
         self.yg_glyph = g
         self.original_axis = self.yg_glyph.current_axis()
         self.new_axis = new_axis
         self.top_window = prefs.top_window()
@@ -2734,24 +2768,24 @@
         """l: a list of ygHint objects"""
         self.undo_stack.push(deleteHintsCommand(self, l))
 
     def set_dirty(self) -> None:
         self._clean = False
         self.yg_font.set_dirty()
 
-    def make_set(
-        self,
-        hint: "ygHint",
-        pt_list: list,
-        touched_point: Optional[ygPoint],
-        callback: Callable,
-    ) -> None:
-        self.undo_stack.push(
-            makeSetCommand(self, hint, pt_list, touched_point, callback)
-        )
+    #def make_set(
+    #    self,
+    #    hint: "ygHint",
+    #    pt_list: list,
+    #    touched_point: Optional[ygPoint],
+    #    callback: Callable,
+    #) -> None:
+    #    self.undo_stack.push(
+    #        makeSetCommand(self, hint, pt_list, touched_point, callback)
+    #    )
 
     def set_clean(self) -> None:
         self._clean = True
 
     def clean(self) -> bool:
         return self._clean
 
@@ -3141,14 +3175,85 @@
                     result.append(vv)
             if index_only:
                 for i, r in enumerate(result):
                     result[i] = self.yg_glyph.resolve_point_identifier(r).index
             return result
         else:
             return [self.yg_glyph.resolve_point_identifier(t).index]
+        
+    def _ptid_to_objects(self):
+        _target_list = self.target_list()
+        pt_list = []
+        for t in _target_list:
+            pt_list.append(self.yg_glyph.resolve_point_identifier(t))
+        return pt_list
+        
+    def contains_points(self, p: Any) -> bool:
+        """Returns True if point p or all points in list p are targets of this hint."""
+        if len(p) == 0:
+            return False
+        pt_list = self._ptid_to_objects()
+        sought_list = []
+        if type(p) is list:
+            for pp in p:
+                sought_list.append(self.yg_glyph.resolve_point_identifier(pp))
+        else:
+            sought_list = [self.yg_glyph.resolve_point_identifier(p)]
+        for p in sought_list:
+            if not p in pt_list:
+                return False
+        return True
+    
+    def _add_points(self, p: list) -> None:
+        """We should already have checked to make sure all points in p are
+        untouched and that this hint is shift, align, or interpolate.
+        Points in p must be type ygPoint."""
+        current_points = self._ptid_to_objects()
+        current_points.extend(p)
+        labels = []
+        for p in current_points:
+            labels.append(p.preferred_label())
+        if len(labels) > 1:
+            self._source["ptid"] = labels
+
+    def add_points(self, p: list) -> None:
+        if self.yg_glyph != None:
+            self.yg_glyph.undo_stack.push(
+                addPointsCommand(self.yg_glyph, self, p)
+            )
+
+    def _delete_points(self, p: list) -> None:
+        if not len(p):
+            return
+        pt_list = self._ptid_to_objects()
+        original_len = len(pt_list)
+        # There's got to be at least one point left for the hint after this operation.
+        if len(p) >= len(pt_list):
+            return
+        for pp in p:
+            ppp = self.yg_glyph.resolve_point_identifier(pp)
+            try:
+                pt_list.remove(ppp)
+            except Exception:
+                pass
+        if len(pt_list) >= original_len:
+            return
+        labels = []
+        for p in pt_list:
+            labels.append(p.preferred_label())
+        if len(labels) == 1:
+            self._source["ptid"] = labels[0]
+        elif len(labels) > 1:
+            self._source["ptid"] = labels
+
+    def delete_points(self, p: list) -> None:
+        if self.yg_glyph != None:
+            self.yg_glyph.undo_stack.push(
+                deletePointsCommand(self.yg_glyph, self, p)
+            )
 
     def ref(self) -> Any:
         if "ref" in self._source:
             return self._source["ref"]
         return None
 
     def set_target(self, tgt: Any) -> None:
```

### Comparing `ygt-0.1.5/src/ygt/ygPreferences.py` & `ygt-0.1.6/src/ygt/ygPreferences.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/ygPreview.py` & `ygt-0.1.6/src/ygt/ygPreview.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,27 @@
         # The height of the glyph above the baseline. Should be able to subtract
         # this from self.ascender to get where on the grid we should start laying
         # down pixels. If the result of the subtraction is negative, we need to
         # display grid above the ascender number.
         self.bitmap_top = 0
         self.grid_height = 0
         self.total_height = 0
-        # self.baseline_position = 0
         # The top of the grid should be offset this far from self.vertical_margin
         self.top_grid_offset = 0
         # The pixels of the glyph start this far down.
         self.top_char_margin = 0
         self.show_grid = True
         # Two- or three-dimensional array shaped by numpy.
         self.Z: list = []
         self.instance_dict: Optional[dict] = None
         self.instance: Optional[str] = None
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
-        bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+        self.background_color = self.palette().color(QPalette.ColorRole.Base)
+        bg_hsv_value = self.background_color.value()
+        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
         self.dark_theme = text_hsv_value > bg_hsv_value
         self.colors = self.mk_color_list()
         self.render_mode = RENDER_LCD_1
         self.hinting_on = True
         self.paintEvent = self.paintEvent_b # type: ignore
 
     def set_up_signal(self, func: Callable) -> None:
@@ -338,18 +339,19 @@
                 painter.drawLine(QLine(left, y_top, left, y_bot))
                 left += self.pixel_size
 
     def paintEvent_a(self, event) -> None:
         """Paint grayscale glyph."""
         painter = QPainter(self)
         brush = QBrush()
-        if self.dark_theme:
-            brush.setColor(QColor("black"))
-        else:
-            brush.setColor(QColor("white"))
+        brush.setColor(self.background_color)
+        #if self.dark_theme:
+        #    brush.setColor(QColor("black"))
+        #else:
+        #    brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
@@ -370,36 +372,40 @@
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
     def paintEvent_b(self, event) -> None:
         """Paint subpixel rendering with solid pixels."""
         painter = QPainter(self)
         brush = QBrush()
-        if self.dark_theme:
-            brush.setColor(QColor("black"))
-        else:
-            brush.setColor(QColor("white"))
+        brush.setColor(self.background_color)
+        #if self.dark_theme:
+        #    brush.setColor(QColor("black"))
+        #else:
+        #    brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
+        black = QColor("black")
         for row in self.Z:
             for col in row:
                 rgb = []
                 for elem in col:
                     rgb.append(elem)
                 if self.dark_theme:
                     qc = QColor(rgb[0], rgb[1], rgb[2])
+                    if qc == black:
+                        qc == self.background_color
                 else:
                     qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
                 qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
                 painter.fillRect(qr, qc)
                 xposition += self.pixel_size
             yposition += self.pixel_size
             xposition = self.horizontal_margin
@@ -408,18 +414,19 @@
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
     def paintEvent_c(self, event) -> None:
         """Paint subpixel rendering with rgb pixel trios."""
         painter = QPainter(self)
         brush = QBrush()
-        if self.dark_theme:
-            brush.setColor(QColor("black"))
-        else:
-            brush.setColor(QColor("white"))
+        brush.setColor(self.background_color)
+        #if self.dark_theme:
+        #    brush.setColor(QColor("black"))
+        #else:
+        #    brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
@@ -494,18 +501,19 @@
                     result.append(yg_font.unicode_to_name[ord(c)])
             except Exception:
                 result.append(".notdef")
         return result
 
     def _fill_background(self, painter: QPainter) -> None:
         brush = QBrush()
-        if self.yg_preview.dark_theme:
-            brush.setColor(QColor("black"))
-        else:
-            brush.setColor(QColor("white"))
+        brush.setColor(self.yg_preview.background_color)
+        #if self.yg_preview.dark_theme:
+        #    brush.setColor(QColor("black"))
+        #else:
+        #    brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
     def paintEvent_a(self, event) -> None:
         target_size = self.yg_preview.char_size
         painter = QPainter(self)
```

### Comparing `ygt-0.1.5/src/ygt/ygSchema.py` & `ygt-0.1.6/src/ygt/ygSchema.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/ygStems.py` & `ygt-0.1.6/src/ygt/ygStems.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt/ygYAMLEditor.py` & `ygt-0.1.6/src/ygt/ygYAMLEditor.py`

 * *Files identical despite different names*

### Comparing `ygt-0.1.5/src/ygt.egg-info/PKG-INFO` & `ygt-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.5
+Version: 0.1.6
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,23 +26,41 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-### Version 0.1.24 (2023-4-19)
+### Version 0.1.6 (2023-4-28)
+
+Select more than one untouched point when adding shift, align, or interpolate hints to create a hint with a set as target. This formerly had to be done with a separate “Make Set” command.
+
+“Make Set” command has been removed as unnecessary.
+
+To add a point to a shift, align, or interpolate hint, select the hint and at least one untouched point, and press the **plus** key.
+
+To delete a point or points from a shift, align, or interpolate hint, select one ore more points belonging to the hint and press the **hyphen** or **minus** key.
+
+Corrected background color of preview panels when dark theme is active.
+
+### Version 0.1.5 (2023-4-25)
+
+Various UI refinements: initial scaling of glyphs, spacebar to temporarily switch to panning mode, and more.
+
+User now confronts only one kind of stem hint: Ygt guesses (more or less accurately) the distance type.
+
+### Version 0.1.4 (2023-4-19)
 
 When we read a UFO, we do not rename glyphs. This prevents incompatibilities between in-memory font and font on disk, and it simplifies export. However, it may complicate shifting back and forth between UFO and YAML modes.
 
 Ygt sometimes hung when summoning a Font View window for fonts read from UFO. This is now fixed.
 
 Program now (partly) honors dark themes on various platforms.
 
-### Version 0.1.23 (2023-4-17)
+### Version 0.1.3 (2023-4-17)
 
 changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
 ```
 s/blackspace/blackdist/g
 s/whitesapce/whitedist/g
 s/grayspace/graydist/g
 ```
```

### Comparing `ygt-0.1.5/src/ygt.egg-info/SOURCES.txt` & `ygt-0.1.6/src/ygt.egg-info/SOURCES.txt`

 * *Files identical despite different names*


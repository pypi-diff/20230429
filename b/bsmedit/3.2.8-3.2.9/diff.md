# Comparing `tmp/bsmedit-3.2.8.tar.gz` & `tmp/bsmedit-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bsmedit-3.2.8.tar", last modified: Wed Nov 23 22:20:29 2022, max compression
+gzip compressed data, was "bsmedit-3.2.9.tar", last modified: Fri Apr 28 18:58:32 2023, max compression
```

## Comparing `bsmedit-3.2.8.tar` & `bsmedit-3.2.9.tar`

### file list

```diff
@@ -1,78 +1,124 @@
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.597841 bsmedit-3.2.8/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     1069 2018-05-21 01:13:05.000000 bsmedit-3.2.8/LICENSE
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       60 2018-08-25 21:13:46.000000 bsmedit-3.2.8/MANIFEST.in
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      356 2022-11-23 22:20:29.593840 bsmedit-3.2.8/PKG-INFO
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.553828 bsmedit-3.2.8/bsmedit/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       96 2020-07-03 22:56:10.000000 bsmedit-3.2.8/bsmedit/__init__.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     1545 2021-12-03 00:21:04.000000 bsmedit-3.2.8/bsmedit/__main__.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.557829 bsmedit-3.2.8/bsmedit/auibarpopup/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      110 2018-07-03 15:56:02.000000 bsmedit-3.2.8/bsmedit/auibarpopup/__init__.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)     5490 2020-07-10 06:17:04.000000 bsmedit-3.2.8/bsmedit/auibarpopup/auibarpopup.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)     6618 2020-07-10 06:17:04.000000 bsmedit-3.2.8/bsmedit/auibarpopup/demo.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.573834 bsmedit-3.2.8/bsmedit/bsm/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       87 2020-05-31 16:56:22.000000 bsmedit-3.2.8/bsmedit/bsm/__init__.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     8135 2020-07-03 22:56:10.000000 bsmedit-3.2.8/bsmedit/bsm/autocomplete.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2420 2018-08-23 04:16:20.000000 bsmedit-3.2.8/bsmedit/bsm/bsm.h
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     1900 2022-10-07 21:14:16.000000 bsmedit-3.2.8/bsmedit/bsm/bsmbackend.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    99551 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/bsm/bsmxpm.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2499 2020-05-31 16:56:12.000000 bsmedit-3.2.8/bsmedit/bsm/csim.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    47713 2020-07-05 07:01:57.000000 bsmedit-3.2.8/bsmedit/bsm/debugger.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     7838 2021-12-16 21:37:48.000000 bsmedit-3.2.8/bsmedit/bsm/debugtool.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    10821 2020-07-03 22:56:10.000000 bsmedit-3.2.8/bsmedit/bsm/dirtreectrl.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2246 2020-05-31 16:56:16.000000 bsmedit-3.2.8/bsmedit/bsm/docstring.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    62938 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/bsm/editor.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    28513 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/bsm/graph.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     8509 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/bsm/lineeditor.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    17549 2021-12-16 04:40:29.000000 bsmedit-3.2.8/bsmedit/bsm/misctools.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     3159 2020-05-31 16:56:23.000000 bsmedit-3.2.8/bsmedit/bsm/pymgr_helpers.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      301 2020-05-31 16:56:23.000000 bsmedit-3.2.8/bsmedit/bsm/pysim.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    36014 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/bsm/shell.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    65252 2021-12-16 21:37:48.000000 bsmedit-3.2.8/bsmedit/bsm/sim.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    32743 2020-05-31 16:56:27.000000 bsmedit-3.2.8/bsmedit/bsm/simprocess.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     3634 2021-12-16 04:40:29.000000 bsmedit-3.2.8/bsmedit/bsm/utility.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2686 2020-05-31 16:51:38.000000 bsmedit-3.2.8/bsmedit/c2p.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.589838 bsmedit-3.2.8/bsmedit/cparser/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      103 2018-06-24 15:52:02.000000 bsmedit-3.2.8/bsmedit/cparser/__init__.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    18673 2018-06-24 15:53:44.000000 bsmedit-3.2.8/bsmedit/cparser/better_exchook.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    13920 2018-06-24 15:52:33.000000 bsmedit-3.2.8/bsmedit/cparser/caching.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)   179673 2018-08-23 04:08:58.000000 bsmedit-3.2.8/bsmedit/cparser/cparser.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      811 2018-06-24 15:51:22.000000 bsmedit-3.2.8/bsmedit/cparser/cparser_utils.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     7012 2018-07-27 06:49:17.000000 bsmedit-3.2.8/bsmedit/cparser/cwrapper.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    16131 2018-06-24 16:13:14.000000 bsmedit-3.2.8/bsmedit/cparser/globalincludewrappers.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     9553 2018-06-24 15:52:20.000000 bsmedit-3.2.8/bsmedit/cparser/goto.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    91026 2018-06-24 16:13:10.000000 bsmedit-3.2.8/bsmedit/cparser/interpreter.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    17271 2018-05-28 22:16:20.000000 bsmedit-3.2.8/bsmedit/cparser/py_demo_unparse.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.589838 bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)     1646 2018-05-28 22:16:20.000000 bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/__init__.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)    27001 2018-05-28 22:16:20.000000 bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sorteddict.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)    75793 2018-05-28 22:16:20.000000 bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sortedlist.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)     9863 2018-05-28 22:16:20.000000 bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sortedset.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    14256 2020-07-09 21:37:18.000000 bsmedit-3.2.8/bsmedit/frameplus.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.589838 bsmedit-3.2.8/bsmedit/glsurface/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      106 2018-06-01 04:22:41.000000 bsmedit-3.2.8/bsmedit/glsurface/__init__.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    14026 2018-06-08 01:47:13.000000 bsmedit-3.2.8/bsmedit/glsurface/_simxpm.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    63377 2020-07-10 06:18:28.000000 bsmedit-3.2.8/bsmedit/glsurface/glsurface.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     4625 2020-05-31 17:12:29.000000 bsmedit-3.2.8/bsmedit/glsurface/gltest.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    16473 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/mainframe.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    45476 2022-10-07 21:14:16.000000 bsmedit-3.2.8/bsmedit/mainframexpm.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.593840 bsmedit-3.2.8/bsmedit/propgrid/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      142 2018-08-23 05:36:36.000000 bsmedit-3.2.8/bsmedit/propgrid/__init__.py
--rwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)    15011 2020-05-31 17:15:47.000000 bsmedit-3.2.8/bsmedit/propgrid/demo.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2144 2020-05-31 17:15:47.000000 bsmedit-3.2.8/bsmedit/propgrid/enumtype.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    25954 2020-05-31 17:15:48.000000 bsmedit-3.2.8/bsmedit/propgrid/formatters.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    27504 2020-05-31 17:15:54.000000 bsmedit-3.2.8/bsmedit/propgrid/prop.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    10261 2020-05-31 17:15:49.000000 bsmedit-3.2.8/bsmedit/propgrid/propart.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    36412 2021-12-16 04:39:59.000000 bsmedit-3.2.8/bsmedit/propgrid/propgrid.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     2507 2020-05-31 18:22:37.000000 bsmedit-3.2.8/bsmedit/propgrid/propxpm.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)    15183 2020-05-31 17:15:57.000000 bsmedit-3.2.8/bsmedit/propgrid/validators.py
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       22 2022-11-23 21:24:34.000000 bsmedit-3.2.8/bsmedit/version.py
-drwxrwxr-x   0 tianzhu   (1000) tianzhu   (1000)        0 2022-11-23 22:20:29.557829 bsmedit-3.2.8/bsmedit.egg-info/
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      356 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/PKG-INFO
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)     1799 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/SOURCES.txt
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)        1 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/dependency_links.txt
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       46 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/entry_points.txt
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       68 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/requires.txt
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)        8 2022-11-23 22:20:29.000000 bsmedit-3.2.8/bsmedit.egg-info/top_level.txt
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      366 2019-12-07 23:16:39.000000 bsmedit-3.2.8/readme.md
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)       38 2022-11-23 22:20:29.597841 bsmedit-3.2.8/setup.cfg
--rw-rw-r--   0 tianzhu   (1000) tianzhu   (1000)      822 2021-12-03 00:21:04.000000 bsmedit-3.2.8/setup.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.983053 bsmedit-3.2.9/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1069 2018-08-26 15:43:59.000000 bsmedit-3.2.9/LICENSE
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       60 2023-03-15 18:35:26.000000 bsmedit-3.2.9/MANIFEST.in
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1652 2023-04-28 18:58:32.980556 bsmedit-3.2.9/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      366 2023-04-28 18:38:39.000000 bsmedit-3.2.9/README.md
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       91 2023-04-28 18:53:22.000000 bsmedit-3.2.9/README_pip.md
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.898020 bsmedit-3.2.9/bsmedit/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       96 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1766 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/__main__.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.905381 bsmedit-3.2.9/bsmedit/aui/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   133330 2023-04-11 21:57:03.000000 bsmedit-3.2.9/bsmedit/aui/AUI.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.914895 bsmedit-3.2.9/bsmedit/aui/aui/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    16175 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/aui/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   170757 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/aui/aui_constants.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    33233 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/aui/aui_switcherdialog.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    20511 2023-04-10 02:31:12.000000 bsmedit-3.2.9/bsmedit/aui/aui/aui_utilities.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   134511 2023-04-06 18:59:43.000000 bsmedit-3.2.9/bsmedit/aui/aui/auibar.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   215623 2023-04-11 21:57:03.000000 bsmedit-3.2.9/bsmedit/aui/aui/auibook.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    48184 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/aui/dockart.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   373654 2023-04-11 21:57:03.000000 bsmedit-3.2.9/bsmedit/aui/aui/framemanager.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   107762 2023-04-11 21:57:03.000000 bsmedit-3.2.9/bsmedit/aui/aui/tabart.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    17917 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/aui/tabmdi.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   510180 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/images.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     4882 2023-04-05 20:43:38.000000 bsmedit-3.2.9/bsmedit/aui/run.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.916752 bsmedit-3.2.9/bsmedit/auibarpopup/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      110 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/auibarpopup/__init__.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     5510 2023-04-07 03:09:08.000000 bsmedit-3.2.9/bsmedit/auibarpopup/auibarpopup.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     6617 2023-04-11 22:20:48.000000 bsmedit-3.2.9/bsmedit/auibarpopup/demo.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.935768 bsmedit-3.2.9/bsmedit/bsm/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       87 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8135 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/autocomplete.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2420 2018-08-26 15:43:59.000000 bsmedit-3.2.9/bsmedit/bsm/bsm.h
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1900 2022-11-23 21:17:13.000000 bsmedit-3.2.9/bsmedit/bsm/bsmbackend.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   107301 2023-04-14 01:18:41.000000 bsmedit-3.2.9/bsmedit/bsm/bsmxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2499 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/csim.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    47667 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/debugger.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8665 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/debugtool.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11788 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/dirtreectrl.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2246 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/docstring.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    43971 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/editor.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    35288 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/editor_base.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    26228 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/graph.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4043 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/graph_common.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    18683 2023-04-15 02:39:50.000000 bsmedit-3.2.9/bsmedit/bsm/graph_datatip.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5876 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/graph_toolbar.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     8319 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/lineeditor.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    36995 2023-04-14 01:18:41.000000 bsmedit-3.2.9/bsmedit/bsm/misctools.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3159 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/pymgr_helpers.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      301 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/bsm/pysim.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    37116 2023-04-28 18:31:41.000000 bsmedit-3.2.9/bsmedit/bsm/shell.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5225 2023-04-28 18:31:41.000000 bsmedit-3.2.9/bsmedit/bsm/shell_base.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    70601 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/sim.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    32743 2023-03-01 01:07:14.000000 bsmedit-3.2.9/bsmedit/bsm/simprocess.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     6878 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/bsm/utility.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2686 2021-12-02 19:00:33.000000 bsmedit-3.2.9/bsmedit/c2p.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.944287 bsmedit-3.2.9/bsmedit/cparser/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      103 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    18673 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/better_exchook.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    13920 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/caching.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)   179673 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/cparser.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      811 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/cparser_utils.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     7012 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/cwrapper.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.946225 bsmedit-3.2.9/bsmedit/cparser/demos/
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     1254 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/demos/interactive_test_parser.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     1153 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/demos/test_interpreter.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    16131 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/globalincludewrappers.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     9553 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/goto.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    91026 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/interpreter.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    17271 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/py_demo_unparse.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.952043 bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     1646 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/__init__.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)    27001 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sorteddict.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)    75793 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sortedlist.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)     9863 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sortedset.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.962677 bsmedit-3.2.9/bsmedit/cparser/tests/
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)      758 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/helpers_test.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2333 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_funcptrdecl.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1798 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_goto.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    93158 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_interpret_stmnt.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1618 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_interpreter_helloworld.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      927 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_parse_func.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4439 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_parse_stmnt.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      226 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_ptrtoptrdecl.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      637 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_sdl_header.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1053 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/cparser/tests/test_simplevardecl.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    14647 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/frameplus.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.965405 bsmedit-3.2.9/bsmedit/glsurface/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      106 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/glsurface/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    14026 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/glsurface/_simxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    63377 2021-12-02 20:48:40.000000 bsmedit-3.2.9/bsmedit/glsurface/glsurface.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     4625 2021-12-02 20:48:40.000000 bsmedit-3.2.9/bsmedit/glsurface/gltest.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    18599 2023-04-12 18:21:15.000000 bsmedit-3.2.9/bsmedit/mainframe.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    45476 2022-11-23 21:17:13.000000 bsmedit-3.2.9/bsmedit/mainframexpm.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.975778 bsmedit-3.2.9/bsmedit/propgrid/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      142 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/propgrid/__init__.py
+-rwxr-xr-x   0 tianzhuqiao   (501) staff       (20)    14027 2023-03-01 00:34:56.000000 bsmedit-3.2.9/bsmedit/propgrid/demo.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2144 2021-12-06 01:32:34.000000 bsmedit-3.2.9/bsmedit/propgrid/enumtype.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    25954 2023-02-24 22:09:21.000000 bsmedit-3.2.9/bsmedit/propgrid/formatters.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    40282 2023-03-09 21:59:39.000000 bsmedit-3.2.9/bsmedit/propgrid/prop.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    11204 2023-02-24 22:09:21.000000 bsmedit-3.2.9/bsmedit/propgrid/propart.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    37776 2023-03-09 22:38:20.000000 bsmedit-3.2.9/bsmedit/propgrid/propgrid.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2507 2018-09-02 04:37:40.000000 bsmedit-3.2.9/bsmedit/propgrid/propxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      292 2023-02-24 22:09:21.000000 bsmedit-3.2.9/bsmedit/propgrid/utility.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)    15265 2023-02-14 16:29:44.000000 bsmedit-3.2.9/bsmedit/propgrid/validators.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      183 2023-04-28 18:58:08.000000 bsmedit-3.2.9/bsmedit/version.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.901788 bsmedit-3.2.9/bsmedit.egg-info/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1652 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/PKG-INFO
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     3035 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/SOURCES.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)        1 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/dependency_links.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       46 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/entry_points.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       68 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/requires.txt
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       41 2023-04-28 18:58:32.000000 bsmedit-3.2.9/bsmedit.egg-info/top_level.txt
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.977078 bsmedit-3.2.9/examples/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     1283 2023-04-14 01:19:04.000000 bsmedit-3.2.9/examples/example.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      814 2023-03-10 19:18:04.000000 bsmedit-3.2.9/examples/start.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.977727 bsmedit-3.2.9/examples/waves/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      454 2018-08-26 15:43:59.000000 bsmedit-3.2.9/examples/waves/setup.py
+drwxr-xr-x   0 tianzhuqiao   (501) staff       (20)        0 2023-04-28 18:58:32.979522 bsmedit-3.2.9/examples/waves/waves/
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      110 2018-08-26 15:43:59.000000 bsmedit-3.2.9/examples/waves/waves/__init__.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     5993 2021-12-02 19:00:33.000000 bsmedit-3.2.9/examples/waves/waves/waves.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)     2649 2018-08-26 15:43:59.000000 bsmedit-3.2.9/examples/waves/waves/wavesxpm.py
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)      784 2023-04-28 18:53:33.000000 bsmedit-3.2.9/pyproject.toml
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       38 2023-04-28 18:58:32.983236 bsmedit-3.2.9/setup.cfg
+-rw-r--r--   0 tianzhuqiao   (501) staff       (20)       69 2023-04-12 18:21:15.000000 bsmedit-3.2.9/setup.py
```

### Comparing `bsmedit-3.2.8/LICENSE` & `bsmedit-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/__main__.py` & `bsmedit-3.2.9/bsmedit/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import multiprocessing
+import ctypes
 import wx
 import click
 from .mainframe import MainFrame
 from .version import __version__
+try:
+    ctypes.windll.shcore.SetProcessDpiAwareness(True)
+except:
+    pass
+
 
 class RunApp(wx.App):
     def __init__(self, **kwargs):
         self.kwargs = kwargs
         wx.App.__init__(self, redirect=False)
 
     def OnInit(self):
@@ -35,20 +41,24 @@
 @click.option('--ignore-perspective',
               '-i',
               is_flag=True,
               help="Do not load perspective.")
 @click.option('--spawn',
               is_flag=True,
               help="Start a process with method 'spawn'.")
+@click.option('--debug',
+              is_flag=True,
+              help='Run in debug mode.')
 @click.argument('module', nargs=-1)
-def main(config, path, ignore_perspective, spawn, module):
+def main(config, path, ignore_perspective, spawn, debug,module):
     if spawn and hasattr(multiprocessing, 'set_start_method'):
         multiprocessing.set_start_method('spawn')
     app = RunApp(config=config,
                  ignore_perspective=ignore_perspective,
                  path=path,
-                 module=module)
+                 module=module,
+                 debug=debug)
     app.MainLoop()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `bsmedit-3.2.8/bsmedit/auibarpopup/auibarpopup.py` & `bsmedit-3.2.9/bsmedit/auibarpopup/auibarpopup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import wx
-import wx.lib.agw.aui as aui
+from bsmedit.aui import aui
 
 class AuiToolBarPopup(wx.Frame):
     def __init__(self, parent):
         wx.Frame.__init__(self, parent, style=wx.NO_BORDER|
                           wx.FRAME_TOOL_WINDOW|wx.FRAME_NO_TASKBAR|
                           wx.FRAME_FLOAT_ON_PARENT|wx.STAY_ON_TOP)
         self._toolbar = None
@@ -51,15 +51,15 @@
             if self._toolbar.GetAuiManager():
                 self._toolbar.GetAuiManager().Update()
             self._toolbar.SetClientSize(sz)
         # refresh the toolbar; otherwise, the status of the radio buttons may
         # not be correct.
         self._toolbar.Refresh()
         self.tb.ClearTools()
-        wx.CallAfter(self.Hide)
+        self.Hide()
 
     def UpdateItems(self, wnd, items):
         items_added = 0
         self._toolbar = wnd
         self.Unbind(wx.EVT_TOOL)
         self.tb.ClearTools()
 
@@ -88,16 +88,16 @@
                     tool.state |= aui.AUI_BUTTON_STATE_CHECKED
             elif item.GetKind() == aui.ITEM_RADIO:
                 tool = self.tb.AddRadioTool(item.GetId(), item.GetLabel(),
                                             item.GetBitmap(), item.GetDisabledBitmap())
                 if item.state & aui.AUI_BUTTON_STATE_CHECKED:
                     tool.state |= aui.AUI_BUTTON_STATE_CHECKED
             elif item.GetKind() == aui.ITEM_NORMAL:
-                tool = self.tb.AddSimpleTool(item.GetId(), item.GetLabel(),
-                                             item.GetBitmap())
+                tool = self.tb.AddTool(item.GetId(), item.GetLabel(),
+                                       item.GetBitmap(), item.GetDisabledBitmap(), aui.ITEM_NORMAL)
                 self.tb.SetToolDropDown(tool.GetId(), wnd.GetToolDropDown(tool.GetId()))
             if tool:
                 tool.SetAlignment(wx.EXPAND)
                 items_added += 1
 
         self.tb.Realize()
         self.SetClientSize(self.tb.GetMinSize())
@@ -122,8 +122,8 @@
         # find out the screen coordinate at the bottom of the tab ctrl
         cli_rect = wnd.GetClientRect()
         pt.y = cli_rect.y + cli_rect.height
         self.popup.Position = wnd.ClientToScreen(pt)
         self.popup.UpdateItems(wnd, items)
         self.popup.Show()
         self.popup.Raise()
-        return -1
+        return None
```

### Comparing `bsmedit-3.2.8/bsmedit/auibarpopup/demo.py` & `bsmedit-3.2.9/bsmedit/auibarpopup/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import wx
-import wx.lib.agw.aui as aui
 import wx.py as py
+from bsmedit.aui import aui
 from auibarpopup import *
 
 ID_TOOL_START = wx.ID_HIGHEST + 1
 
 class MyPanel(wx.Panel):
     def __init__(self, parent, *args, **kwargs):
         wx.Panel.__init__(self, parent, *args, **kwargs)
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/autocomplete.py` & `bsmedit-3.2.9/bsmedit/bsm/autocomplete.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/bsm.h` & `bsmedit-3.2.9/bsmedit/bsm/bsm.h`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/bsmbackend.py` & `bsmedit-3.2.9/bsmedit/bsm/bsmbackend.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/bsmxpm.py` & `bsmedit-3.2.9/bsmedit/bsm/bsmxpm.py`

 * *Files 10% similar despite different names*

```diff
@@ -5479,29 +5479,252 @@
 "  y n.C C B V S B * T R W.3 3 . ",
 "  q n.P _ ) ( / ^ + Q W.W.W.E . ",
 "  e r.J J H P C H O < > W.> 3 . ",
 "  0 C.r.r.9.q.9.C.I % 1 E 1 % . ",
 "    5 5 9 6 5 8 8 5 # o . X @   "
 ]
 
-forward_svg = '<svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><path d="M0,0h24v24H0V0z" fill="none"/></g><g><polygon points="6.23,20.23 8,22 18,12 8,2 6.23,3.77 14.46,12"/></g></svg>'
-backward_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none" opacity=".87"/><path d="M17.51 3.87L15.73 2.1 5.84 12l9.9 9.9 1.77-1.77L9.38 12l8.13-8.13z"/></svg>'
+wand_xpm = [
+"16 16 71 1 ",
+"  c None",
+". c #151515",
+"X c #161616",
+"o c gray9",
+"O c #313131",
+"+ c #353535",
+"@ c #373737",
+"# c gray22",
+"$ c #3E3E3E",
+"% c #3F3F3F",
+"& c gray25",
+"* c gray26",
+"= c #434343",
+"- c gray27",
+"; c gray28",
+": c #4C4C4C",
+"> c gray30",
+", c #4E4E4E",
+"< c gray31",
+"1 c #585858",
+"2 c #676767",
+"3 c DimGray",
+"4 c #F1B100",
+"5 c #F1B300",
+"6 c #F1B500",
+"7 c #F1B700",
+"8 c #F1B900",
+"9 c #F2B70D",
+"0 c #F1BC08",
+"q c #F3BD11",
+"w c #F3BD13",
+"e c #F3BF17",
+"r c #F2BD19",
+"t c #F3BF19",
+"y c #F5C125",
+"u c #F5C127",
+"i c #F5C32B",
+"p c #F5C52F",
+"a c #B49741",
+"s c #BFA14B",
+"d c #C2A44E",
+"f c #C2A54F",
+"g c #CDB05A",
+"h c #CFB15B",
+"j c #DCBF68",
+"k c #F6CA41",
+"l c #F5CC4B",
+"z c #F6CD4B",
+"x c #F7CE4E",
+"c c #F7CE50",
+"v c #F6CF51",
+"b c #F7D05A",
+"n c #F7D66A",
+"m c #F8D76D",
+"M c #F8D974",
+"N c #F8D977",
+"B c #F8DC7D",
+"V c #818181",
+"C c #838383",
+"Z c #848484",
+"A c gray55",
+"S c #959595",
+"D c #A9A9A9",
+"F c #F8DD83",
+"G c gray79",
+"H c #CACACA",
+"J c LightGray",
+"K c gray87",
+"L c gray97",
+"P c #F8F8F8",
+"I c #FEFEFE",
+"                ",
+"          i     ",
+"       piyc t   ",
+"        bmBxw   ",
+"     iyxFdhjk08 ",
+"       xdPIgn7  ",
+"      e<HLJsM7  ",
+"     w<2ADaN57  ",
+"     <2#*<lt9   ",
+"    <2@*.55 5   ",
+"   1C@$.  5     ",
+"  ;C@$.         ",
+" *C@$.          ",
+"3KO=.           ",
+"3HS.            ",
+" $.             "
+]
+
+refresh_xpm = [
+"16 16 88 1 ",
+"  c None",
+". c #23611F",
+"X c #246320",
+"o c #256522",
+"O c #276623",
+"+ c #296824",
+"@ c #2A6B26",
+"# c #2C6D27",
+"$ c #32742C",
+"% c #33762E",
+"& c #377B32",
+"* c #3A7E34",
+"= c #3C8035",
+"- c #3E8337",
+"; c #408639",
+": c #42883B",
+"> c #448B3D",
+", c #4A8B45",
+"< c #4C8D47",
+"1 c #499141",
+"2 c #4D9645",
+"3 c #4F9947",
+"4 c #4F9049",
+"5 c #51924B",
+"6 c #54954E",
+"7 c #519B49",
+"8 c #539E4B",
+"9 c #569750",
+"0 c #55A14D",
+"q c #57A34E",
+"w c #5AA650",
+"e c #5EAB54",
+"r c #5FAD56",
+"t c #62A25B",
+"y c #63A45D",
+"u c #65A75E",
+"i c #65B45B",
+"p c #67B65C",
+"a c #68B95E",
+"s c #6ABB5F",
+"d c #68A860",
+"f c #68AA61",
+"g c #6BAC63",
+"h c #6CAD65",
+"j c #6EB066",
+"k c #6CBC60",
+"l c #6DBE62",
+"z c #76B36F",
+"x c #7CBD73",
+"c c #7EBF75",
+"v c #6EC063",
+"b c #7FC179",
+"n c #81BE7A",
+"m c #81C277",
+"M c #83C379",
+"N c #82C27A",
+"B c #83C479",
+"V c #85C77B",
+"C c #85C47E",
+"Z c #87C480",
+"A c #89C380",
+"S c #8BC383",
+"D c #8AC483",
+"F c #89C682",
+"G c #8BC683",
+"H c #8BC785",
+"J c #8DC786",
+"K c #8EC686",
+"L c #8EC985",
+"P c #8FC987",
+"I c #8FC988",
+"U c #90CA88",
+"Y c #92CA89",
+"T c #91CA8A",
+"R c #94CB8C",
+"E c #95CC8D",
+"W c #96CD8F",
+"Q c #98CE8F",
+"! c #99CF90",
+"~ c #9ACF92",
+"^ c #9CCF94",
+"/ c #9CD094",
+"( c #9ED195",
+") c #9FD196",
+"_ c #9FD297",
+"` c #A1D298",
+"' c #A4D49B",
+"] c #A7D79E",
+"                ",
+"         31     ",
+"    iiw82dt*    ",
+"  aMU///RLD6#   ",
+" pL'Q~EUDCb<o   ",
+" c`^Ju;=%4,X    ",
+"eAED>=   O.     ",
+"031:=           ",
+"           031:=",
+"     lk   82KIz%",
+"    lVMew7gSIF9 ",
+"   lB]'_~RLMCy@ ",
+"   ic)^WRFnh5+  ",
+"    qjf:-&$#    ",
+"     1:         ",
+"                "
+]
+
+forward_svg = '<svg xmlns="http://www.w3.org/2000/svg"  height="24px" viewBox="0 0 24 24" width="24px" fill="#32a1e6" stroke-width="1" stroke="#32a1e6"><polygon points="6.23,20.23 8,22 18,12 8,2 6.23,3.77 14.46,12"/></svg>'
+forward_disable_svg = '<svg xmlns="http://www.w3.org/2000/svg"  height="24px" viewBox="0 0 24 24" width="24px" fill="#8E8E93" stroke-width="1" stroke="#8E8E93"><polygon points="6.23,20.23 8,22 18,12 8,2 6.23,3.77 14.46,12"/></svg>'
+backward_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#32a1e6" stroke-width="1" stroke="#32a1e6"><path d="M17.51 3.87L15.73 2.1 5.84 12l9.9 9.9 1.77-1.77L9.38 12l8.13-8.13z"/></svg>'
+backward_disable_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#8E8E93" stroke-width="1" stroke="#8E8E93"><path d="M17.51 3.87L15.73 2.1 5.84 12l9.9 9.9 1.77-1.77L9.38 12l8.13-8.13z"/></svg>'
 
 radio_unchecked_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#8E8E93"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8z"/></svg>'
 radio_disabled_svg = '<svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="48px" viewBox="0 0 24 24" width="48px" fill="#8E8E93"><g><rect fill="none" height="24" width="24"/></g><g><g><path d="M12,2C6.47,2,2,6.47,2,12s4.47,10,10,10s10-4.47,10-10S17.53,2,12,2z"/></g></g></svg>'
 radio_checked_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#8E8E93"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8z"/><circle cx="12" cy="12" r="5"/></svg>'
 radio_activated_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#FF9500"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8z"/><circle cx="12" cy="12" r="5"/></svg>'
 
-run_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/></svg>'
+run_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/></svg>'
 run_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/></svg>'
-stop_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#007AFF" ><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><rect height="14" rx="0" width="14" x="5" y="5"/></svg>'
+stop_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#32a1e6" ><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><rect height="14" rx="0" width="14" x="5" y="5"/></svg>'
 stop_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#8E8E93" ><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><rect height="14" rx="0" width="14" x="5" y="5"/></svg>'
-pause_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><g><rect height="16" rx="0" width="4" x="6" y="4"/><rect height="16" rx="0" width="4" x="14" y="4"/></g></svg>'
+pause_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><g><rect height="16" rx="0" width="4" x="6" y="4"/><rect height="16" rx="0" width="4" x="14" y="4"/></g></svg>'
 pause_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><g><rect height="16" rx="0" width="4" x="6" y="4"/><rect height="16" rx="0" width="4" x="14" y="4"/></g></svg>'
-step_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/><rect height="16" rx="0" width="4 " x="16" y="4"/></svg>'
+step_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/><rect height="16" rx="0" width="4 " x="16" y="4"/></svg>'
 step_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" width="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M5,20 l14 -8 L5,4 V14 z"/><rect height="16" rx="0" width="4 " x="16" y="4"/></svg>'
-step_over_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,14A2,2 0 0,1 14,16A2,2 0 0,1 12,18A2,2 0 0,1 10,16A2,2 0 0,1 12,14M23.46,8.86L21.87,15.75L15,14.16L18.8,11.78C17.39,9.5 14.87,8 12,8C8.05,8 4.77,10.86 4.12,14.63L2.15,14.28C2.96,9.58 7.06,6 12,6C15.58,6 18.73,7.89 20.5,10.72L23.46,8.86Z" /></svg>'
+step_over_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,14A2,2 0 0,1 14,16A2,2 0 0,1 12,18A2,2 0 0,1 10,16A2,2 0 0,1 12,14M23.46,8.86L21.87,15.75L15,14.16L18.8,11.78C17.39,9.5 14.87,8 12,8C8.05,8 4.77,10.86 4.12,14.63L2.15,14.28C2.96,9.58 7.06,6 12,6C15.58,6 18.73,7.89 20.5,10.72L23.46,8.86Z" /></svg>'
 step_over_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,14A2,2 0 0,1 14,16A2,2 0 0,1 12,18A2,2 0 0,1 10,16A2,2 0 0,1 12,14M23.46,8.86L21.87,15.75L15,14.16L18.8,11.78C17.39,9.5 14.87,8 12,8C8.05,8 4.77,10.86 4.12,14.63L2.15,14.28C2.96,9.58 7.06,6 12,6C15.58,6 18.73,7.89 20.5,10.72L23.46,8.86Z" /></svg>'
-step_into_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,2V13L17.5,8.5L18.92,9.92L12,16.84L5.08,9.92L6.5,8.5L11,13V2H13Z" /></svg>'
+step_into_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,2V13L17.5,8.5L18.92,9.92L12,16.84L5.08,9.92L6.5,8.5L11,13V2H13Z" /></svg>'
 step_into_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)" /><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,2V13L17.5,8.5L18.92,9.92L12,16.84L5.08,9.92L6.5,8.5L11,13V2H13Z" /></svg>'
-step_out_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#007AFF"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)"/><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,16H11V6L6.5,10.5L5.08,9.08L12,2.16L18.92,9.08L17.5,10.5L13,6V16Z" /></svg>'
+step_out_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#32a1e6"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)"/><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,16H11V6L6.5,10.5L5.08,9.08L12,2.16L18.92,9.08L17.5,10.5L13,6V16Z" /></svg>'
 step_out_grey_svg = '<svg xmlns="http://www.w3.org/2000/svg" width="48px" height="48px" viewBox="0 0 24 24" fill="#8E8E93"><rect width="24" height="24" style="fill:none;stroke-width:0;stroke:rgb(0,0,0)"/><path d="M12,22A2,2 0 0,1 10,20A2,2 0 0,1 12,18A2,2 0 0,1 14,20A2,2 0 0,1 12,22M13,16H11V6L6.5,10.5L5.08,9.08L12,2.16L18.92,9.08L17.5,10.5L13,6V16Z" /></svg>'
+
+file_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 96 960 960" width="48" fill="#32a1e6"><path d="M319 806h322v-60H319v60Zm0-170h322v-60H319v60Zm-99 340q-24 0-42-18t-18-42V236q0-24 18-42t42-18h361l219 219v521q0 24-18 42t-42 18H220Zm331-554V236H220v680h520V422H551ZM220 236v186-186 680-680Z"/></svg>'
+
+input_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48"fill="#32a1e6"><path d="M190 785 l-86-86 219-219-219-219 86-86 305 305-305 305Z"/><path d="M740 30v900h120v-900h-120Z"/><circle cx="545" cy="480" r="120"/></svg>'
+
+output_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" fill="#32a1e6"><path d="M380 785 l-86-86 219-219-219-219 86-86 305 305-305 305Z"/><path d="M100 30v900h120v-900h-120Z"/><circle cx="740" cy="480" r="120"/></svg>'
+
+inout_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" fill="#32a1e6"><path d="M580 785 l-86-86 219-219-219-219 86-86 305 305-305 305Z"/><path d="M380 785 l86-86 -219-219 219-219 -86-86 -305 305 305 305Z"/><path d="M440 30v900h80v-900h-80Z"/><circle cx="840" cy="480" r="120"/><circle cx="120" cy="480" r="120"/></svg>'
+
+signal_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" fill="#32a1e6"><path d="M580 785 l-86-86 219-219-219-219 86-86 305 305-305 305Z"/><path d="M380 785 l86-86 -219-219 219-219 -86-86 -305 305 305 305Z"/><circle cx="840" cy="480" r="120"/><circle cx="120" cy="480" r="120"/></svg>'
+
+module_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" fill="#32a1e6" stroke="#32a1e6"><rect fill="none" stroke-width="120" x="30" y="30" width="900" height="900" /><circle cx="240" cy="240" r="120"/><circle cx="720" cy="720" r="120"/><circle cx="240" cy="720" r="120"/><circle cx="480" cy="480" r="120"/></svg>'
+
+setting_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 96 960 960" width="48" fill="#32a1e6" stroke="#32a1e6" stroke-width="50"><path d="m388 976-20-126q-19-7-40-19t-37-25l-118 54-93-164 108-79q-2-9-2.5-20.5T185 576q0-9 .5-20.5T188 535L80 456l93-164 118 54q16-13 37-25t40-18l20-127h184l20 126q19 7 40.5 18.5T669 346l118-54 93 164-108 77q2 10 2.5 21.5t.5 21.5q0 10-.5 21t-2.5 21l108 78-93 164-118-54q-16 13-36.5 25.5T592 850l-20 126H388Zm92-270q54 0 92-38t38-92q0-54-38-92t-92-38q-54 0-92 38t-38 92q0 54 38 92t92 38Zm0-60q-29 0-49.5-20.5T410 576q0-29 20.5-49.5T480 506q29 0 49.5 20.5T550 576q0 29-20.5 49.5T480 646Zm0-70Zm-44 340h88l14-112q33-8 62.5-25t53.5-41l106 46 40-72-94-69q4-17 6.5-33.5T715 576q0-17-2-33.5t-7-33.5l94-69-40-72-106 46q-23-26-52-43.5T538 348l-14-112h-88l-14 112q-34 7-63.5 24T306 414l-106-46-40 72 94 69q-4 17-6.5 33.5T245 576q0 17 2.5 33.5T254 643l-94 69 40 72 106-46q24 24 53.5 41t62.5 25l14 112Z"/></svg>'
+
+more_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" fill="#32a1e6"><circle cy="800" cx="480" r="100"/><circle cy="480" cx="480" r="100"/><circle cy="160" cx="480" r="100"/></svg>'
+
+home_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 0 960 960" width="48" stroke-width="50" stroke="#32a1e6" fill="#32a1e6"><path  d="M120 876        h200v-300h320v300h200v-490L480 91 120 386v490Zm-60 60v-580l420 -340 420 340v580h-320v-300h-200v300h-320Zm370-353Z"/></svg>'
+
+up_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48px" viewBox="0 0 24 24" width="48px" fill="#32a1e6" stroke-width="1" stroke="#32a1e6"><path d="M3.87 17.51 L2.1 15.73 12 5.84 l9.9 9.9 -1.77 1.77L12 9.38 l-8.13 8.13z"/></svg>'
+
+new_page_svg = '<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 96 960 960" width="48" fill="#32a1e6"><path d="M180 936q-24.75 0-42.375-17.625T120 876V276q0-24.75 17.625-42.375T180 216h600q24.75 0 42.375 17.625T840 276v329q-14-8-29.5-13t-30.5-8V276H180v600h309q4 16 9.023 31.172Q503.045 922.345 510 936H180Zm0-107v47-600 308-4 249Zm100-53h211q4-16 9-31t13-29H280v60Zm0-170h344q14-7 27-11.5t29-8.5v-40H280v60Zm0-170h400v-60H280v60Zm452.5 579q-77.5 0-132.5-55.5T545 828q0-78.435 54.99-133.718Q654.98 639 733 639q77 0 132.5 55.282Q921 749.565 921 828q0 76-55.5 131.5t-133 55.5ZM718 955h33V845h110v-33H751V702h-33v110H608v33h110v110Z"/></svg>'
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/csim.py` & `bsmedit-3.2.9/bsmedit/bsm/csim.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/debugger.py` & `bsmedit-3.2.9/bsmedit/bsm/debugger.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import time
 import inspect  #for debugger frame inpsection
 import sys  #for set_trace etc
 import os.path  #for absolute filename conversions
 import ctypes  #for pythonapi calls
 from codeop import _maybe_compile, Compile
 import traceback  #for formatting errors
+import six.moves._thread as thread  #for keyboard interrupt
 import wx
 import wx.py.dispatcher as dp
-import six.moves._thread as thread  #for keyboard interrupt
+from .shell_base import magic
 
 help_msg = """
 \"\"\"
 #help | #h:
     - show this text.
 #step | #s:
     - step to the next line.
@@ -32,15 +33,15 @@
     - quit the debugger.
 #stop:
     - interrupt the execution
 \"\"\"
 """
 
 
-class PseudoEvent(object):
+class PseudoEvent:
     """
     An object with the same interface as a threading.Event for the internal
     engine. This prevents the readline/readlines and debugger from blocking
     when waiting for user input.
 
     This calls the doyield function and sleeps until the event is set.
     """
@@ -60,19 +61,20 @@
             wx.YieldIfNeeded()
             # send the EVT_UPDATE_UI events so the UI status has a chance to
             # update (e.g., menubar, toolbar)
             wx.EventLoop.GetActive().ProcessIdle()
             time.sleep(0.05)
 
 
-class EngineDebugger(object):
+class EngineDebugger:
     bpnum = 0
 
-    def __init__(self):
+    def __init__(self, use_magic=True):
         self.compiler = EngineCompiler()
+        self.use_magic = use_magic
         #debugger state
         self._paused = False  #is paused.
         self._can_stepin = False  #debugger is about to enter a new scope
         self._can_stepout = False  #debugger can be stepped out of a scope
 
         #debugger command flags
         self._resume = False  #debugging was resumed.
@@ -412,15 +414,15 @@
         return True
 
     def get_status(self):
         """return the current status"""
         if self._active_scope < 0 or self._active_scope >= len(self._frames):
             return None
         frame = self._frames[self._active_scope]
-        filename = inspect.getsourcefile(frame) or inspect.getfile(frame)
+        filename = frame.f_code.co_filename
         lineno = frame.f_lineno
         name = frame.f_code.co_name
         return {
             'name': name,
             'filename': self._abs_filename(filename),
             'lineno': lineno,
             'scopes': self._scopes,
@@ -540,15 +542,15 @@
         #check if the debugger want to end debugging.
         if self._end is True:
             sys.settrace(None)
             #use a blank trace function as returning None doesn't work
             return self._trace_off
 
         #file and name of scope being called.
-        filename = inspect.getsourcefile(frame) or inspect.getfile(frame)
+        filename = frame.f_code.co_filename
         lineno = frame.f_lineno
 
         #if the file is on the block list do not trace
         #this is mainly engine/message bus files and prevents the user pausing and
         #locking the engine communications.
         if self._check_files(filename, self._block_files):
             return None
@@ -607,15 +609,15 @@
         if self._end is True:
             sys.settrace(None)
             #use a blank trace function as returning None doesn't work
             #this is a python bug (as of python2.7 01/2011)
             return self._trace_off
 
         #file and name of scope being called.
-        filename = inspect.getsourcefile(frame) or inspect.getfile(frame)
+        filename = frame.f_code.co_filename
         lineno = frame.f_lineno
 
         #check for breakpoints
         filename = self._abs_filename(filename)
         bps = self.bpoints.filter(('filename', 'lineno'), (filename, lineno))
         for bpdata in bps:
             paused = self._hit_bp(bpdata, frame)
@@ -651,15 +653,15 @@
         #check if the debugger want to end debugging.
         if self._end is True:
             sys.settrace(None)
             #use a blank trace function as returning None doesn't work
             return self._trace_off
 
         #file and name of scope being called.
-        filename = inspect.getsourcefile(frame) or inspect.getfile(frame)
+        filename = frame.f_code.co_filename
         lineno = frame.f_lineno
 
         #check for breakpoints
         filename = self._abs_filename(filename)
         bps = self.bpoints.filter(('filename', 'lineno'), (filename, lineno))
         for bpdata in bps:
             will_break = self._check_bp(bpdata, frame)
@@ -687,15 +689,15 @@
         else:
             self._can_stepout = False
             self._can_stepin = True
         if event == 'call' and not self._stepin:
             return
 
         # do not stop inside the system files
-        filename = inspect.getsourcefile(frame) or inspect.getfile(frame)
+        filename = frame.f_code.co_filename
         for f in sys.path + ['<input>', '<string>']:
             if filename.startswith(f):
                 return
 
         #send a paused message to the console
         #(it will publish an ENGINE_DEBUG_PAUSED message after updating internal
         #state)
@@ -726,14 +728,16 @@
             #user command to process.
             else:
                 line = self._cmd
                 self._cmd = None
                 #check for debugger commands
                 handled = self._process_dbg_command(line)
                 if handled is False:
+                    if self.use_magic:
+                        line = magic(line)
                     #not a command so execute as python source
                     self._process_dbg_source(line)
 
         #reset stepin flag
         self._can_stepin = False
 
         ##Debugger will run next line
@@ -834,16 +838,15 @@
         scopes = []
         frames = []
         #loop backwards through frames until the bottom frame and generate lists
         #of scope names and frames.
         while frame is not None:
             name = frame.f_code.co_name
             if name == '<module>':
-                filename = inspect.getsourcefile(frame) or inspect.getfile(
-                    frame)
+                filename = frame.f_code.co_filename
                 if filename == '<input>':
                     name = 'Main'
             scopes.append(name)
             frames.append(frame)
 
             #check the next frame back
             if frame == self._bottom_frame:
@@ -1027,23 +1030,22 @@
 
         ##run the code in the active scope
         _, frame, g, l = self.get_scope(self._active_scope)
         try:
             exec(code, g, l)
         except SystemExit:
             self.write_debug('Blocking system exit')
-        except KeyboardInterrupt:
+        except KeyboardInterrupt as exc:
             self._paused = False
-            raise KeyboardInterrupt
+            raise KeyboardInterrupt from exc
         except:
             #engine wanted to stop anyway - probably wxPython keyboard interrupt error
             if self._stop is True:
                 self._paused = False
                 raise KeyboardInterrupt
-
             #error in user code.
             self.compiler.show_traceback()
 
         #update the locals
         self._update_frame_locals(frame)
 
         ##Finished running the code - prompt for a new command
@@ -1068,15 +1070,15 @@
 """
 
 
 # A general purpose list type object used for storing dictionaries these can
 # then be filtered by key.
 # Used to store breakpoints in both the engine debugger (engine process) and
 # engine manager(gui process) where breakpoints are stored as dictionaries
-class DictList(object):
+class DictList:
     def __init__(self, dicts=None, default=None):
         """
         Create a list like container object for dictionaries with the ability to
         look up dicts by key value or by index.
 
         dicts - is a sequence of dictionaries to populate the DictList with.
         default - a defualt dictionary to use to create a new dictionary in the
@@ -1373,15 +1375,15 @@
                     #alter line number
                     tblist[n] = (filename, lineno + self._lineadjust, offset,
                                  line)
                 lst = traceback.format_list(tblist)
                 if lst:
                     lst.insert(0, "Traceback (most recent call last):\n")
                 lst[len(lst):] = traceback.format_exception_only(typ, value)
-            map(sys.stderr.write, lst)
+            print(''.join(lst).strip())
         except:
             pass
 
     # Message handlers
     def future_flag(self, msg):
         """enable or disable a __future__ feature using flags"""
         flag, is_set = msg.get_data()
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/debugtool.py` & `bsmedit-3.2.9/bsmedit/bsm/debugtool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import inspect
+import os
 import six
 import wx
 import wx.py.dispatcher as dp
 import wx.lib.mixins.listctrl as listmix
-import wx.lib.agw.aui as aui
+from ..aui import aui
 from .bsmxpm import (run_svg, run_grey_svg, step_over_svg, step_over_grey_svg, step_into_svg, \
-                     step_into_grey_svg, step_out_svg, step_out_grey_svg, step_over_svg, stop_svg, stop_grey_svg)
+                     step_into_grey_svg, step_out_svg, step_out_grey_svg, stop_svg, stop_grey_svg)
 
 from .utility import svg_to_bitmap
+from ..auibarpopup import AuiToolBarPopupArt
 
 class StackListCtrl(wx.ListCtrl, listmix.ListCtrlAutoWidthMixin,
                     listmix.ListRowHighlighter):
     def __init__(self, *args, **kwargs):
         wx.ListCtrl.__init__(self, *args, **kwargs)
 
         listmix.ListCtrlAutoWidthMixin.__init__(self)
@@ -22,15 +23,15 @@
 class StackPanel(wx.Panel):
     def __init__(self, parent):
         wx.Panel.__init__(self, parent)
         sizer = wx.BoxSizer(wx.VERTICAL)
         self.listctrl = StackListCtrl(self,
                                       style=wx.LC_REPORT
                                       | wx.BORDER_NONE
-                                      | wx.LC_EDIT_LABELS | wx.LC_VRULES
+                                      | wx.LC_VRULES
                                       | wx.LC_HRULES | wx.LC_SINGLE_SEL)
         # | wx.BORDER_SUNKEN
         # | wx.LC_SORT_ASCENDING
         # | wx.LC_NO_HEADER
         self.listctrl.InsertColumn(0, 'Name')
         self.listctrl.InsertColumn(1, 'Line')
         self.listctrl.InsertColumn(2, 'File')
@@ -38,19 +39,26 @@
         self.SetSizer(sizer)
         self.Bind(wx.EVT_LIST_ITEM_ACTIVATED, self.OnItemActivated,
                   self.listctrl)
         dp.connect(self.OnDebugEnded, 'debugger.ended')
         dp.connect(self.OnDebugUpdateScopes, 'debugger.update_scopes')
         dp.connect(self.OnDebugUpdateScopes, 'debugger.paused')
 
+        self.frames = []
+
+        self.show_all_frames = False
+        resp = dp.send('frame.get_config', group='debugtool', key='show_all_frames')
+        if resp and resp[0][1] is not None:
+            self.show_all_frames = resp[0][1]
+
     def Destroy(self):
         dp.disconnect(self.OnDebugEnded, 'debugger.ended')
         dp.disconnect(self.OnDebugUpdateScopes, 'debugger.update_scopes')
         dp.disconnect(self.OnDebugUpdateScopes, 'debugger.paused')
-        super(StackPanel, self).Destroy()
+        super().Destroy()
 
     def OnDebugEnded(self):
         """debugger is ended"""
         # clear the scopes
         self.listctrl.DeleteAllItems()
 
     def OnDebugUpdateScopes(self):
@@ -58,40 +66,51 @@
         self.listctrl.DeleteAllItems()
         resp = dp.send(signal='debugger.get_status')
         if not resp or not resp[0][1]:
             return
         status = resp[0][1]
         frames = status['frames']
         level = status['active_scope']
+        self.frames = []
         if frames is not None:
-            for frame in frames:
+            for l, frame in enumerate(reversed(frames)):
                 name = frame.f_code.co_name
-                filename = inspect.getsourcefile(frame) or inspect.getfile(
-                    frame)
+                filename = frame.f_code.co_filename
                 lineno = frame.f_lineno
+                if not self.show_all_frames and filename == '<input>':
+                    break
                 index = self.listctrl.InsertItem(six.MAXSIZE, name)
-                self.listctrl.SetItem(index, 2, filename)
-                self.listctrl.SetItem(index, 1, '%d' % lineno)
-        if level >= 0 and level < self.listctrl.GetItemCount():
-            self.listctrl.SetItemTextColour(level, 'blue')
+                filename_short = os.path.relpath(filename)
+                if len(filename_short) > len(filename):
+                    filename_short = filename
+                self.listctrl.SetItem(index, 2, filename_short)
+                self.listctrl.SetItem(index, 1, f'{lineno}')
+                self.frames.append([name, filename, lineno, len(frames)-1-l])
+                self.listctrl.SetItemData(index, len(self.frames)-1)
+        level_idx = len(frames)-1-level
+        if 0 <= level_idx < self.listctrl.GetItemCount():
+            self.listctrl.SetItemTextColour(level_idx, 'blue')
         self.listctrl.RefreshRows()
 
     def OnItemActivated(self, event):
-        currentItem = event.m_itemIndex
-        filename = self.listctrl.GetItem(currentItem, 2).GetText()
-        lineno = self.listctrl.GetItem(currentItem, 1).GetText()
+        item = event.GetIndex()
+        index = self.listctrl.GetItemData(item)
+        if 0 <=  index < len(self.frames):
+            _, filename, lineno, level = self.frames[index]
+        else:
+            return
         # open the script first
         dp.send(signal='frame.file_drop',
                 filename=filename,
                 lineno=int(lineno))
         # ask the debugger to trigger the update scope event to set mark
-        dp.send(signal='debugger.set_scope', level=currentItem)
+        dp.send(signal='debugger.set_scope', level=level)
 
 
-class DebugTool(object):
+class DebugTool():
     isInitialized = False
     frame = None
     showStackPanel = True
 
     @classmethod
     def Initialize(cls, frame, **kwargs):
         if cls.isInitialized:
@@ -107,15 +126,16 @@
                 showhidemenu='View:Panels:Call Stack')
 
         # debugger toolbar
         dp.send('frame.add_menu',
                 path='Tools:Debug',
                 rxsignal='',
                 kind='Popup')
-        cls.tbDebug = aui.AuiToolBar(frame, style=wx.TB_FLAT | wx.TB_HORIZONTAL)
+        cls.tbDebug = aui.AuiToolBar(frame, agwStyle=aui.AUI_TB_OVERFLOW)
+        cls.toolbarart = AuiToolBarPopupArt(frame)
         items = (
             ('Run\tF5', 'resume', run_svg, run_grey_svg, 'paused'),
             ('Stop\tShift-F5', 'stop', stop_svg, stop_grey_svg, 'paused'),
             ('Step\tF10', 'step', step_over_svg, step_over_grey_svg, 'paused'),
             ('Step Into\tF11', 'step_into', step_into_svg, step_into_grey_svg, 'can_stepin'),
             ('Step Out\tShift-F11', 'step_out', step_out_svg, step_out_grey_svg, 'can_stepout'),
         )
@@ -124,16 +144,17 @@
             resp = dp.send('frame.add_menu',
                            path='Tools:Debug:' + label,
                            rxsignal='debugger.' + signal,
                            updatesignal='debugtool.updateui')
             if not resp:
                 continue
             cls.menus[resp[0][1]] = status
-            cls.tbDebug.AddTool(resp[0][1], label, svg_to_bitmap(xpm),
-                                svg_to_bitmap(xpm_grey), wx.ITEM_NORMAL, label)
+            cls.tbDebug.AddTool(resp[0][1], label, svg_to_bitmap(xpm, win=cls.tbDebug),
+                                svg_to_bitmap(xpm_grey, win=cls.tbDebug), wx.ITEM_NORMAL, label)
+        cls.tbDebug.SetArtProvider(cls.toolbarart)
         cls.tbDebug.Realize()
 
         dp.send('frame.add_panel',
                 panel=cls.tbDebug,
                 title='Debugger',
                 active=False,
                 paneInfo=aui.AuiPaneInfo().Name('debugger').Caption(
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/dirtreectrl.py` & `bsmedit-3.2.9/bsmedit/bsm/dirtreectrl.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,31 @@
 
 
     @todo:
         extract ico from exes found in directory
 """
 
 import os
+import platform
+import stat
 import traceback
+import fnmatch
 import wx
 
 
+def is_hidden(filepath):
+    filepath = os.path.abspath(filepath)
+    name = os.path.basename(filepath)
+    if platform.system() == 'Darwin':       # macOS
+        return name.startswith('.')
+    elif platform.system() == 'Windows':    # Windows
+        return bool(os.stat(filepath).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN)
+    else:                                   # linux variants
+        return name.startswith('.')
+
 class Directory(object):
     """Simple class for using as the data object in the DirTreeCtrl"""
     __name__ = 'Directory'
 
     def __init__(self, directory=''):
         self.directory = directory
 
@@ -60,23 +73,24 @@
         self.iconentries = {}
         self.imagelist = wx.ImageList(16, 16)
 
         # blank default
         self.iconentries['default'] = -1
         self.iconentries['directory'] = -1
         self.iconentries['directoryopen'] = -1
-        self.addBitmap(
-            wx.ArtProvider.GetBitmap(wx.ART_FOLDER, wx.ART_OTHER, (16, 16)),
-            'directory')
-        self.addBitmap(
-            wx.ArtProvider.GetBitmap(wx.ART_FOLDER_OPEN, wx.ART_OTHER,
-                                     (16, 16)), 'directoryopen')
-        self.addBitmap(
-            wx.ArtProvider.GetBitmap(wx.ART_NORMAL_FILE, wx.ART_OTHER,
-                                     (16, 16)), 'default')
+        scale = self.GetContentScaleFactor()
+        bmp = wx.ArtProvider.GetBitmap(wx.ART_FOLDER, wx.ART_OTHER, (16*scale, 16*scale))
+        bmp.SetScaleFactor(scale)
+        self.addBitmap(bmp, 'directory')
+        bmp = wx.ArtProvider.GetBitmap(wx.ART_FOLDER_OPEN, wx.ART_OTHER, (16*scale, 16*scale))
+        bmp.SetScaleFactor(scale)
+        self.addBitmap(bmp, 'directoryopen')
+        bmp = wx.ArtProvider.GetBitmap(wx.ART_NORMAL_FILE, wx.ART_OTHER, (16*scale, 16*scale))
+        bmp.SetScaleFactor(scale)
+        self.addBitmap(bmp, 'default')
         self.SetImageList(self.imagelist)
         # # you should replace this with your own code or put the relevant
         # # images in the correct path # set directory image
         # self.addIcon('images/folder.png', wx.BITMAP_TYPE_PNG, 'directory')
         #
         # # set default image
         # self.addIcon('images/page.png', wx.BITMAP_TYPE_PNG, 'default')
@@ -90,31 +104,31 @@
 
     def addIcon(self, filepath, wxBitmapType, name):
         """Adds an icon to the imagelist and registers it with the iconentries dict
         using the given name. Use so that you can assign custom icons to the tree
         just by passing in the value stored in self.iconentries[name]
         @param filepath: path to the image
         @param wxBitmapType: wx constant for the file type - eg wx.BITMAP_TYPE_PNG
-        @param name: name to use as a key in the self.iconentries dict - get your imagekey by calling
-            self.iconentries[name]
+        @param name: name to use as a key in the self.iconentries dict -
+                     get your imagekey by calling self.iconentries[name]
         """
         try:
             if os.path.exists(filepath):
                 key = self.imagelist.Add(wx.Bitmap(filepath, wxBitmapType))
                 self.iconentries[name] = key
         except:
             traceback.print_exc()
 
     def SetDeleteOnCollapse(self, selection):
         """Sets the tree option to delete leaf items when the node is
         collapsed. Will slow down the tree slightly but will probably save memory."""
         if isinstance(selection, bool):
             self.DELETEONCOLLAPSE = selection
 
-    def SetRootDir(self, directory):
+    def SetRootDir(self, directory, pattern=None, show_hidden=True):
         """Sets the root directory for the tree. Throws an exception
         if the directory is invalid.
         @param directory: directory to load
         """
 
         # check if directory exists and is a directory
         if not os.path.isdir(directory):
@@ -128,17 +142,17 @@
         self.SetItemData(root, Directory(directory))
         self.SetItemImage(root, self.iconentries['directory'],
                           wx.TreeItemIcon_Normal)
         self.SetItemImage(root, self.iconentries['directoryopen'],
                           wx.TreeItemIcon_Expanded)
         #self.Expand(root)
         # load items
-        self._loadDir(root, directory)
+        self._loadDir(root, directory, pattern=pattern, show_hidden=show_hidden)
 
-    def _loadDir(self, item, directory):
+    def _loadDir(self, item, directory, pattern=None, show_hidden=True):
         """Private function that gets called to load the file list
         for the given directory and append the items to the tree.
         Throws an exception if the directory is invalid.
 
         @note: does not add items if the node already has children"""
 
         # check if directory exists and is a directory
@@ -154,14 +168,20 @@
             # add directory nodes to tree
             for f in files:
                 # if directory, tell tree it has children
                 if os.path.isdir(os.path.join(directory, f)):
                     folders_all.append(f)
                 else:
                     files_all.append(f)
+            if pattern:
+                files_all = fnmatch.filter(files_all, pattern)
+            if not show_hidden:
+                folders_all = [f for f in folders_all if not is_hidden(f)]
+                files_all = [f for f in files_all if not is_hidden(f)]
+
             folders_all.sort(key=lambda y: y.lower())
             files_all.sort(key=lambda y: y.lower())
             for f in folders_all:
                 # process the file extension to build image list
                 imagekey = self.processFileExtension(os.path.join(
                     directory, f))
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/docstring.py` & `bsmedit-3.2.9/bsmedit/bsm/docstring.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/editor.py` & `bsmedit-3.2.9/bsmedit/bsm/editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import os
-import inspect
 import keyword
 import pprint
 import six
+import numpy as np
 import wx
-import wx.stc as stc
+from wx import stc
 import wx.py.dispatcher as dp
-import wx.lib.agw.aui as aui
+from ..aui import aui
 from ..auibarpopup import AuiToolBarPopupArt
 from .bsmxpm import open_xpm, save_xpm, saveas_xpm, find_xpm, indent_xpm, \
                     dedent_xpm, run_xpm, execute_xpm, check_xpm, debug_xpm, \
                     folder_xpm, vert_xpm, horz_xpm, reload_xpm
 from .pymgr_helpers import Gcm
 from .. import to_byte
+from .utility import get_file_finder_name, show_file_in_finder
+from .editor_base import *
 
 
 class BreakpointSettingsDlg(wx.Dialog):
     def __init__(self, parent, condition='', hitcount='', curhitcount=0):
         wx.Dialog.__init__(self,
                            parent,
                            title="Breakpoint Condition",
-                           size=wx.Size(431, 290),
+                           size=wx.DefaultSize,
                            style=wx.DEFAULT_DIALOG_STYLE | wx.RESIZE_BORDER)
 
-        self.SetSizeHintsSz(wx.DefaultSize, wx.DefaultSize)
+        #self.SetSizeHints(wx.DefaultSize, wx.DefaultSize)
         szAll = wx.BoxSizer(wx.VERTICAL)
         label = ('When the breakkpoint location is reached, the expression is '
-                 'evaluated and the breakpoint is hit only if the expression '
+                 'evaluated, and the breakpoint is hit only if the expression '
                  'is true.')
         self.stInfo = wx.StaticText(self, label=label)
-        self.stInfo.Wrap(-1)
-        szAll.Add(self.stInfo, 1, wx.ALL, 15)
-        szCnd = wx.BoxSizer(wx.HORIZONTAL)
+        self.stInfo.SetMaxSize((420, -1))
+        self.stInfo.Wrap(420)
+        szAll.Add(self.stInfo, 0, wx.ALL|wx.EXPAND, 15)
 
-        szCnd.AddSpacer((20, 0), 0, wx.EXPAND, 5)
+        szCnd = wx.BoxSizer(wx.HORIZONTAL)
+        szCnd.Add(20, 0, 0)
 
         szCond = wx.BoxSizer(wx.VERTICAL)
-
         self.cbCond = wx.CheckBox(self, label="Is true")
         szCond.Add(self.cbCond, 0, wx.ALL | wx.EXPAND, 5)
 
         self.tcCond = wx.TextCtrl(self, wx.ID_ANY)
         szCond.Add(self.tcCond, 0, wx.ALL | wx.EXPAND, 5)
 
         label = "Hit count (hit count: #; for example, #>10"
@@ -50,38 +52,39 @@
         self.tcHitCount = wx.TextCtrl(self, wx.ID_ANY)
         szCond.Add(self.tcHitCount, 0, wx.ALL | wx.EXPAND, 5)
         label = "Current hit count: %d" % curhitcount
         self.stHtCount = wx.StaticText(self, label=label)
         szCond.Add(self.stHtCount, 0, wx.ALL | wx.EXPAND, 5)
 
         szCnd.Add(szCond, 1, wx.EXPAND, 5)
-
-        szAll.Add(szCnd, 1, wx.EXPAND, 5)
+        szCnd.Add(20, 0, 0)
+        szAll.Add(szCnd, 0, wx.EXPAND, 5)
 
         self.stLine = wx.StaticLine(self, style=wx.LI_HORIZONTAL)
         szAll.Add(self.stLine, 0, wx.EXPAND | wx.ALL, 5)
 
-        szConfirm = wx.BoxSizer(wx.HORIZONTAL)
+        btnsizer = wx.StdDialogButtonSizer()
 
-        self.btnOK = wx.Button(self, wx.ID_OK, "OK")
-        szConfirm.Add(self.btnOK, 0, wx.ALL, 5)
+        self.btnOK = wx.Button(self, wx.ID_OK)
+        self.btnOK.SetDefault()
+        btnsizer.AddButton(self.btnOK)
 
-        self.btnCancel = wx.Button(self, wx.ID_CANCEL, "Cancel")
-        szConfirm.Add(self.btnCancel, 0, wx.ALL, 5)
+        self.btnCancel = wx.Button(self, wx.ID_CANCEL)
+        btnsizer.AddButton(self.btnCancel)
+        btnsizer.Realize()
 
-        szAll.Add(szConfirm, 0, wx.ALIGN_RIGHT, 5)
-
-        self.SetSizer(szAll)
-        self.Layout()
+        szAll.Add(btnsizer, 0, wx.ALIGN_RIGHT, 5)
 
         # initialize the controls
         self.condition = condition
         self.hitcount = hitcount
         self.SetSizer(szAll)
         self.Layout()
+        szAll.Fit(self)
+
         if self.condition == '':
             self.cbCond.SetValue(False)
             self.tcCond.Disable()
         else:
             self.cbCond.SetValue(True)
         self.tcCond.SetValue(self.condition)
         if self.hitcount == '':
@@ -113,171 +116,157 @@
             self.hitcount = ""
         event.Skip()
 
     def GetCondition(self):
         return (self.condition, self.hitcount)
 
 
-NUM_MARGIN = 0
-MARK_MARGIN = 1
-FOLD_MARGIN = 2
-
-
-class PyEditor(wx.py.editwindow.EditWindow):
+class PyEditor(EditorBase):
     ID_COMMENT = wx.NewId()
     ID_UNCOMMENT = wx.NewId()
     ID_EDIT_BREAKPOINT = wx.NewId()
     ID_DELETE_BREAKPOINT = wx.NewId()
     ID_CLEAR_BREAKPOINT = wx.NewId()
 
-    def __init__(self, parent, style=wx.CLIP_CHILDREN | wx.BORDER_NONE):
-        wx.py.editwindow.EditWindow.__init__(self, parent, style=style)
-        self.SetUpEditor()
-        # disable the auto-insert the call tip
-        self.callTipInsert = False
-        self.filename = ""
-        self.autoCompleteKeys = [ord('.')]
-        rsp = dp.send('shell.auto_complete_keys')
-        if rsp:
-            self.autoCompleteKeys = rsp[0][1]
+    def __init__(self, parent):
+        super().__init__(parent)
+
+        self.break_point_candidate = None
+
         self.breakpointlist = {}
-        self.highlightStr = ""
-        self.SetMouseDwellTime(500)
 
-        # Assign handlers for keyboard events.
-        self.Bind(wx.EVT_CHAR, self.OnChar)
-        self.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_LEFT_UP, self.OnLeftUp)
-        self.Bind(stc.EVT_STC_MARGINCLICK, self.OnMarginClick)
-        self.Bind(stc.EVT_STC_DOUBLECLICK, self.OnDoubleClick)
-        self.Bind(stc.EVT_STC_DWELLSTART, self.OnMouseDwellStart)
-        self.Bind(stc.EVT_STC_DWELLEND, self.OnMouseDwellEnd)
-        # Assign handler for the context menu
-        self.Bind(wx.EVT_CONTEXT_MENU, self.OnContextMenu)
-        self.Bind(wx.EVT_UPDATE_UI, self.OnUpdateCommandUI)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent)
+    def OnMotion(self, event):
+        super().OnMotion(event)
+        event.Skip()
+
+        dc = wx.ClientDC(self)
+        pos = event.GetLogicalPosition(dc)
 
-        self.CmdKeyAssign(ord('Z'), wx.stc.STC_SCMOD_CTRL, wx.stc.STC_CMD_UNDO)
-        self.CmdKeyAssign(ord('Z'), wx.stc.STC_SCMOD_CTRL | wx.stc.STC_SCMOD_SHIFT, wx.stc.STC_CMD_REDO)
+        c, x, y = self.HitTest(pos)
+        if self.break_point_candidate:
+            self.MarkerDeleteHandle(self.break_point_candidate)
+        if x == 0 and self.MarkerGet(y) & 2**0 == 0:
+            style = self.GetStyleAt(self.XYToPosition(x, y))
+            if style in [stc.STC_P_COMMENTLINE, stc.STC_P_COMMENTBLOCK]:
+                return
+            txt = self.GetLine(y)
+            txt = txt.strip()
+            if txt and txt[0] != '#':
+                self.break_point_candidate = self.MarkerAdd(y, MARKER_BP_CANDIDATE)
 
     def ClearBreakpoint(self):
         """clear all the breakpoint"""
         for key in list(self.breakpointlist):
             ids = self.breakpointlist[key]['id']
             dp.send('debugger.clear_breakpoint', id=ids)
 
-    def SaveFile(self, filename):
-        """save file"""
-        if super(PyEditor, self).SaveFile(filename):
-            # remember the filename
-            fname = os.path.abspath(filename)
-            fname = os.path.normcase(fname)
-            self.filename = fname
-            return True
-        return False
+    def findBreakPoint(self, line):
+        for key in self.breakpointlist:
+            if line == self.MarkerLineFromHandle(key):
+                return self.breakpointlist[key]
+        return None
 
-    def LoadFile(self, filename):
-        """load file into editor"""
-        self.ClearBreakpoint()
-        if super(PyEditor, self).LoadFile(filename):
-            # remember the filename
-            fname = os.path.abspath(filename)
-            fname = os.path.normcase(fname)
-            self.filename = fname
-            return True
-        return False
+    def comment(self):
+        """Comment section"""
+        self.prepandText('##')
 
-    def OnKillFocus(self, event):
-        """lose focus"""
-        # close the autocomplete and calltip windows
-        if self.CallTipActive():
-            self.CallTipCancel()
-        # crash on mac
-        #if self.AutoCompActive():
-        #    self.AutoCompCancel()
-        event.Skip()
+    def uncomment(self):
+        """Uncomment section"""
+        self.deprepandText('##')
 
-    def OnChar(self, event):
+    def GetContextMenu(self):
         """
-        Keypress event handler.
-
-        Only receives an event if OnKeyDown calls event.Skip() for the
-        corresponding event.
+            Create and return a context menu for the shell.
+            This is used instead of the scintilla default menu
+            in order to correctly respect our immutable buffer.
         """
-        key = event.GetKeyCode()
-        currpos = self.GetCurrentPos()
-        line = self.GetCurrentLine()
-        stoppos = self.PositionFromLine(line)
-        # Return (Enter) needs to be ignored in this handler.
-        if key in [wx.WXK_RETURN, wx.WXK_NUMPAD_ENTER]:
-            pass
-        elif key in self.autoCompleteKeys:
-            # Usually the dot (period) key activates auto completion.
-            # Get the command between the prompt and the cursor.  Add
-            # the autocomplete character to the end of the command.
-            if self.AutoCompActive():
-                self.AutoCompCancel()
-            command = self.GetTextRange(stoppos, currpos) + chr(key)
-            self.AddText(chr(key))
-            if self.autoComplete:
-                self.autoCompleteShow(command)
-        elif key == ord('('):
-            # The left paren activates a call tip and cancels an
-            # active auto completion.
-            if self.AutoCompActive():
-                self.AutoCompCancel()
-            # Get the command between the prompt and the cursor.  Add
-            # the '(' to the end of the command.
-            self.ReplaceSelection("""""")
-            command = self.GetTextRange(stoppos, currpos) + '('
-            self.AddText('(')
-            self.autoCallTipShow(command,
-                                 self.GetCurrentPos() == self.GetTextLength())
-        else:
-            # Allow the normal event handling to take place.
-            event.Skip()
+        menu = super().GetContextMenu()
 
-    def OnKeyDown(self, event):
-        """key down"""
-        key = event.GetKeyCode()
-        control = event.ControlDown()
-        # shift=event.ShiftDown()
-        alt = event.AltDown()
-        if key == wx.WXK_RETURN and not control and not alt \
-            and not self.AutoCompActive():
-            # auto-indentation
-            if self.CallTipActive():
-                self.CallTipCancel()
-            line = self.GetCurrentLine()
-            txt = self.GetLine(line)
-            pos = self.GetCurrentPos()
-            linePos = self.PositionFromLine(line)
-            self.CmdKeyExecute(stc.STC_CMD_NEWLINE)
-            indent = self.GetLineIndentation(line)
-            tabWidth = max(1, self.GetTabWidth())
-            if self.GetUseTabs():
-                indentation = '\t'
+        menu.AppendSeparator()
+        menu.Append(self.ID_COMMENT, 'Comment')
+        menu.Append(self.ID_UNCOMMENT, 'Uncomment')
+        return menu
+
+    def OnContextMenu(self, evt):
+        p = self.ScreenToClient(evt.GetPosition())
+        m = self.GetMarginWidth(0) + self.GetMarginWidth(1)
+        if p.x > m:
+            # show edit menu when the mouse is in editable area
+            menu = self.GetContextMenu()
+            self.PopupMenu(menu)
+        elif p.x > self.GetMarginWidth(0):
+            # in breakpoint area
+            cline = self.LineFromPosition(self.PositionFromPoint(p))
+            for key in self.breakpointlist:
+                line = self.MarkerLineFromHandle(key)
+                if line == cline:
+                    self.GotoLine(line)
+                    break
             else:
-                indentation = ' ' * tabWidth
-            padding = indentation * (int(indent / tabWidth))
-            newpos = self.GetCurrentPos()
-            # smart indentation
-            stripped = txt[:pos - linePos].split('#')[0].strip()
-            firstWord = stripped.split(' ')[0]
-            if stripped and self.needsIndent(firstWord, lastChar=stripped[-1]):
-                padding += indentation
-            elif self.needsDedent(firstWord):
-                padding = padding[:-tabWidth]
-            self.InsertText(newpos, padding)
-            newpos += len(padding)
-            self.SetCurrentPos(newpos)
-            self.SetSelection(newpos, newpos)
-        else:
-            event.Skip()
+                return
+            menu = wx.Menu()
+            menu.Append(self.ID_DELETE_BREAKPOINT, 'Delete Breakpoint')
+            menu.AppendSeparator()
+            menu.Append(self.ID_EDIT_BREAKPOINT, 'Condition...')
+            menu.AppendSeparator()
+            menu.Append(self.ID_CLEAR_BREAKPOINT, 'Delete All Breakpoints')
+            self.PopupMenu(menu)
+
+    def SetupEditor(self):
+        """
+        This method carries out the work of setting up the demo editor.
+        It's separate so as not to clutter up the init code.
+        """
+        super().SetupEditor()
+
+        # key binding
+        self.CmdKeyAssign(ord('R'), stc.STC_SCMOD_CTRL, stc.STC_CMD_REDO)
+        if wx.Platform == '__WXMAC__':
+            self.CmdKeyAssign(ord('R'), wx.stc.STC_SCMOD_META, wx.stc.STC_CMD_REDO)
+
+        self.SetLexer(stc.STC_LEX_PYTHON)
+        # add '.' to wordchars, so in mouse dwell event, it will capture variable
+        # 'a.b'
+        self.SetWordChars('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_.')
+        keywords = list(keyword.kwlist)
+        for key in ['None', 'True', 'False']:
+            if key in keywords:
+                keywords.remove(key)
+        self.SetKeyWords(0, ' '.join(keywords))
+        self.SetKeyWords(1, ' '.join(['None', 'True', 'False']))
+
+        # Set up the numbers in the margin for margin #1
+        self.SetMarginType(NUM_MARGIN, stc.STC_MARGIN_NUMBER)
+        # Reasonable value for, say, 4-5 digits using a mono font (40 pix)
+        self.SetMarginWidth(0, 50)
+
+        # Margin #1 - breakpoint symbols
+        self.SetMarginType(MARK_MARGIN, stc.STC_MARGIN_SYMBOL)
+        # do not show fold symbols
+        self.SetMarginMask(MARK_MARGIN, ~stc.STC_MASK_FOLDERS)
+        self.SetMarginSensitive(MARK_MARGIN, True)
+        self.SetMarginWidth(MARK_MARGIN, 12)
+
+        # Setup a margin to hold fold markers
+        self.SetMarginType(FOLD_MARGIN, stc.STC_MARGIN_SYMBOL)
+        self.SetMarginMask(FOLD_MARGIN, stc.STC_MASK_FOLDERS)
+        self.SetMarginSensitive(FOLD_MARGIN, True)
+        self.SetMarginWidth(FOLD_MARGIN, 12)
+
+        self.SetCaretLineBackAlpha(64)
+        self.SetCaretLineVisible(True)
+        self.SetCaretLineVisibleAlways(True)
+
+        theme = 'solarized-dark'
+        resp = dp.send('frame.get_config', group='editor', key='theme')
+        if resp and resp[0][1] is not None:
+            theme = resp[0][1]
+
+        self.SetupColor(theme)
+        self.SetupColorPython(theme)
 
     def OnMarginClick(self, evt):
         """left mouse button click on margin"""
         margin = evt.GetMargin()
         ctrldown = evt.GetControl()
         # set/edit/delete a breakpoint
         if margin in [NUM_MARGIN, MARK_MARGIN]:
@@ -341,23 +330,19 @@
 
     def OnMouseDwellStart(self, event):
         resp = dp.send(signal='debugger.get_status')
         if not resp or not resp[0][1]:
             return
 
         pos = event.GetPosition()
-        #line = self.LineFromPosition(pos) # 0, 1, 2
         if pos == -1:
             return
-        c = self.GetWordChars()
-        self.SetWordChars(c + '.')
         WordStart = self.WordStartPosition(pos, True)
         WordEnd = self.WordEndPosition(pos, True)
         text = self.GetTextRange(WordStart, WordEnd)
-        self.SetWordChars(c)
         try:
             status = resp[0][1]
             frames = status['frames']
             level = status['active_scope']
             frame = frames[level]
             f_globals = frame.f_globals
             f_locals = frame.f_locals
@@ -428,436 +413,20 @@
                         if self.GetFoldExpanded(line):
                             self.SetFoldExpanded(line, True)
                     line = self.Expand(line, do_expand, force, vis_levels - 1)
             else:
                 line = line + 1
         return line
 
-    def OnDoubleClick(self, event):
-        """left mouse button double click"""
-        # highlight all the instances of the selected text
-        sel = self.GetSelectedText()
-        if sel != "":
-            self.highlightText(sel)
-
-        event.Skip()
-
-    def OnLeftUp(self, event):
-        """left mouse button released"""
-        # remove the highlighting when click somewhere else
-        sel = self.GetSelectedText()
-        if self.highlightStr != "" and sel != self.highlightStr:
-            self.highlightText(self.highlightStr, False)
-
-        event.Skip()
-
-    def highlightText(self, strWord, highlight=True):
-        """highlight the text"""
-        current = 0
-        position = -1
-        flag = stc.STC_FIND_WHOLEWORD | stc.STC_FIND_MATCHCASE
-        if not highlight:
-            self.IndicatorClearRange(0, self.GetLength())
-            self.highlightStr = ""
-            return
-
-        self.highlightStr = strWord
-        self.SetIndicatorCurrent(0)
-        while True:
-            position = self.FindText(current, len(self.GetText()), strWord,
-                                     flag)
-            if isinstance(position, tuple):
-                position = position[0] # wx ver 4.1.0 returns (start, end)
-            current = position + len(strWord)
-            if position == -1:
-                break
-            self.IndicatorFillRange(position, len(strWord))
-
-    def needsIndent(self, firstWord, lastChar):
-        '''Tests if a line needs extra indenting, i.e., if, while, def, etc '''
-        # remove trailing ":" on token
-        if firstWord and firstWord[-1] == ':':
-            firstWord = firstWord[:-1]
-        # control flow keywords
-        keys = [
-            'for', 'if', 'else', 'def', 'class', 'elif', 'try', 'except',
-            'finally', 'while', 'with'
-        ]
-        return firstWord in keys and lastChar == ':'
-
-    def needsDedent(self, firstWord):
-        '''Tests if a line needs extra dedenting, i.e., break, return, etc '''
-        # control flow keywords
-        return firstWord in ['break', 'return', 'continue', 'yield', 'raise']
-
-    def autoCompleteShow(self, command, offset=0):
-        """Display auto-completion popup list."""
-        self.AutoCompSetAutoHide(self.autoCompleteAutoHide)
-        self.AutoCompSetIgnoreCase(self.autoCompleteCaseInsensitive)
-
-        options = []
-        # retrieve the auto complete list from shell
-        response = dp.send('shell.auto_complete_list', command=command)
-        if response:
-            options = response[0][1]
-        if options:
-            self.AutoCompShow(offset, ' '.join(options))
-
-    def autoCallTipShow(self, command, insertcalltip=True, forceCallTip=False):
-        """Display argument spec and docstring in a popup window."""
-        if self.CallTipActive():
-            self.CallTipCancel()
-        (argspec, tip) = (None, None)
-        # retrieve the all tip from shell
-        response = dp.send('shell.auto_call_tip', command=command)
-        if response:
-            # name, argspec, tip
-            (_, argspec, tip) = response[0][1]
-        if tip:
-            dp.send('Shell.calltip', sender=self, calltip=tip)
-        if not self.autoCallTip and not forceCallTip:
-            return
-        startpos = self.GetCurrentPos()
-        if argspec and insertcalltip and self.callTipInsert:
-            self.AddText(argspec + ')')
-            endpos = self.GetCurrentPos()
-            self.SetSelection(startpos, endpos)
-        if argspec:
-            tippos = startpos
-            fallback = startpos - self.GetColumn(startpos)
-            # In case there isn't enough room, only go back to the
-            # fallback.
-            tippos = max(tippos, fallback)
-            self.CallTipShow(tippos, argspec)
-
-    # Some methods to make it compatible with how the wxTextCtrl is used
-    def SetValue(self, value):
-        # if wx.USE_UNICODE:
-        #    value = value.decode('iso8859_1')
-        val = self.GetReadOnly()
-        self.SetReadOnly(False)
-        self.SetText(value)
-        self.EmptyUndoBuffer()
-        self.SetSavePoint()
-        self.SetReadOnly(val)
-
-    def SelectLine(self, line):
-        """select the line"""
-        start = self.PositionFromLine(line)
-        end = self.GetLineEndPosition(line)
-        self.SetSelection(start, end)
-
-    def UpdateStatusText(self):
-        """update the info on statusbar"""
-        caretPos = self.GetCurrentPos()
-        col = self.GetColumn(caretPos) + 1
-        line = self.LineFromPosition(caretPos) + 1
-        dp.send('frame.show_status_text',
-                text='%d, %d' % (line, col),
-                index=1,
-                width=100)
-
-    def OnUpdateUI(self, event):
-        super(PyEditor, self).OnUpdateUI(event)
-        wx.CallAfter(self.UpdateStatusText)
-
-    def SetUpEditor(self):
-        """
-        This method carries out the work of setting up the demo editor.
-        It's separate so as not to clutter up the init code.
-        """
-        # key binding
-        self.CmdKeyAssign(ord('R'), stc.STC_SCMOD_CTRL, stc.STC_CMD_REDO)
-        self.SetLexer(stc.STC_LEX_PYTHON)
-        keywords = keyword.kwlist
-        keywords.extend(['None', 'as', 'True', 'False'])
-        self.SetKeyWords(0, ' '.join(keywords))
-        # Enable folding
-        self.SetProperty('fold', '1')
-        # Highlight tab/space mixing (shouldn't be any)
-        self.SetProperty('tab.timmy.whinge.level', '1')
-        # Set left and right margins
-        self.SetMargins(2, 2)
-        # Set up the numbers in the margin for margin #1
-        self.SetMarginType(NUM_MARGIN, stc.STC_MARGIN_NUMBER)
-        # Reasonable value for, say, 4-5 digits using a mono font (40 pix)
-        self.SetMarginWidth(0, 50)
-        # Indentation and tab stuff
-        self.SetIndent(4)
-        self.SetIndentationGuides(True)
-        # Backspace unindents rather than delete 1 space
-        self.SetBackSpaceUnIndents(True)
-        self.SetTabIndents(True)
-
-        # Use spaces rather than tabs, or TabTimmy will complain!
-        self.SetUseTabs(False)
-        # Don't view white space
-        self.SetViewWhiteSpace(False)
-        # EOL: Since we are loading/saving ourselves, and the
-        # strings will always have \n's in them, set the STC to
-        # edit them that way.
-        self.SetEOLMode(stc.STC_EOL_LF)
-        self.SetViewEOL(False)
-        # No right-edge mode indicator
-        self.SetEdgeMode(stc.STC_EDGE_NONE)
-        # Margin #1 - breakpoint symbols
-        self.SetMarginType(MARK_MARGIN, stc.STC_MARGIN_SYMBOL)
-        # do not show fold symbols
-        self.SetMarginMask(MARK_MARGIN, ~stc.STC_MASK_FOLDERS)
-        self.SetMarginSensitive(MARK_MARGIN, True)
-        self.SetMarginWidth(MARK_MARGIN, 12)
-        # break point
-        self.MarkerDefine(0, stc.STC_MARK_CIRCLE, '#8E8E93', '#FF3B30')
-        # paused at marker
-        self.MarkerDefine(1, stc.STC_MARK_SHORTARROW, '#8E8E93', '#34C759')
-        self.MarkerDefine(2, stc.STC_MARK_SHORTARROW, '#8E8E93', 'WHITE')
-
-        # Setup a margin to hold fold markers
-        self.SetMarginType(FOLD_MARGIN, stc.STC_MARGIN_SYMBOL)
-        self.SetMarginMask(FOLD_MARGIN, stc.STC_MASK_FOLDERS)
-        self.SetMarginSensitive(FOLD_MARGIN, True)
-        self.SetMarginWidth(FOLD_MARGIN, 12)
-        # and now set up the fold markers
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDEREND,
-                          stc.STC_MARK_BOXPLUSCONNECTED, 'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDEROPENMID,
-                          stc.STC_MARK_BOXMINUSCONNECTED, 'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDERMIDTAIL, stc.STC_MARK_TCORNER,
-                          'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDERTAIL, stc.STC_MARK_LCORNER,
-                          'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDERSUB, stc.STC_MARK_VLINE,
-                          'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDER, stc.STC_MARK_BOXPLUS,
-                          'white', '#8E8E93')
-        self.MarkerDefine(stc.STC_MARKNUM_FOLDEROPEN, stc.STC_MARK_BOXMINUS,
-                          'white', '#8E8E93')
-        # Global default style
-        if wx.Platform == '__WXMSW__':
-            self.StyleSetSpec(stc.STC_STYLE_DEFAULT,
-                              'fore:#1D1D1D,back:#FFFFFF,face:Courier New')
-        elif wx.Platform == '__WXMAC__':
-            # TODO: if this looks fine on Linux too, remove the Mac-specific case
-            # and use this whenever OS != MSW.
-            self.StyleSetSpec(stc.STC_STYLE_DEFAULT,
-                              'fore:#1D1D1D,back:#FFFFFF,face:Monaco')
-        else:
-            #defsize = \
-            #    wx.SystemSettings.GetFont(wx.SYS_ANSI_FIXED_FONT).GetPointSize()
-            defsize = 14
-            self.StyleSetSpec(
-                stc.STC_STYLE_DEFAULT,
-                'fore:#000000,back:#FFFFFF,face:Courier,size:%d' % defsize)
-        # Clear styles and revert to default.
-        self.StyleClearAll()
-        # Following style specs only indicate differences from default.
-        # The rest remains unchanged.
-        # Line numbers in margin
-        self.StyleSetSpec(stc.STC_STYLE_LINENUMBER,
-                          'fore:#3C3C43,back:#F2F2F7')
-        # Highlighted brace
-        self.StyleSetSpec(stc.STC_STYLE_BRACELIGHT,
-                          'fore:#00009D,back:#FFFF00')
-        # Unmatched brace
-        self.StyleSetSpec(stc.STC_STYLE_BRACEBAD, 'fore:#00009D,back:#FF0000')
-        # Indentation guide
-        self.StyleSetSpec(stc.STC_STYLE_INDENTGUIDE, 'fore:#CDCDCD')
-        # Python styles
-        self.StyleSetSpec(stc.STC_P_DEFAULT, 'fore:#000000')
-        # Comments
-        self.StyleSetSpec(stc.STC_P_COMMENTLINE, 'fore:#008000,back:#F0FFF0')
-        self.StyleSetSpec(stc.STC_P_COMMENTBLOCK, 'fore:#008000,back:#F0FFF0')
-        # Numbers
-        self.StyleSetSpec(stc.STC_P_NUMBER, 'fore:#008080')
-        # Strings and characters
-        self.StyleSetSpec(stc.STC_P_STRING, 'fore:#800080')
-        self.StyleSetSpec(stc.STC_P_CHARACTER, 'fore:#800080')
-        # Keywords
-        self.StyleSetSpec(stc.STC_P_WORD, 'fore:#000080,bold')
-        # Triple quotes
-        self.StyleSetSpec(stc.STC_P_TRIPLE, 'fore:#800080,back:#FFFFEA')
-        self.StyleSetSpec(stc.STC_P_TRIPLEDOUBLE, 'fore:#800080,back:#FFFFEA')
-        # Class names
-        self.StyleSetSpec(stc.STC_P_CLASSNAME, 'fore:#0000FF,bold')
-        # Function names
-        self.StyleSetSpec(stc.STC_P_DEFNAME, 'fore:#008080,bold')
-        # Operators
-        self.StyleSetSpec(stc.STC_P_OPERATOR, 'fore:#800000,bold')
-        # Identifiers. I leave this as not bold because everything seems
-        # to be an identifier if it doesn't match the above criterae
-        self.StyleSetSpec(stc.STC_P_IDENTIFIER, 'fore:#000000')
-        # Caret color
-        self.SetCaretForeground('#007AFF')
-        # Selection background
-        self.SetSelBackground(1, '#66CCFF')
-        self.SetSelBackground(
-            True, wx.SystemSettings.GetColour(wx.SYS_COLOUR_HIGHLIGHT))
-        self.SetSelForeground(
-            True, wx.SystemSettings.GetColour(wx.SYS_COLOUR_HIGHLIGHTTEXT))
-        self.SetWrapMode(stc.STC_WRAP_WORD)
-        # indicator
-        self.IndicatorSetStyle(0, stc.STC_INDIC_ROUNDBOX)
-        self.IndicatorSetForeground(0, '#FF3B30')
-
-    def prepandText(self, text):
-        """Comment section"""
-        doc = self
-        sel = doc.GetSelection()
-        start = doc.LineFromPosition(sel[0])
-        end = doc.LineFromPosition(sel[1])
-        end_pos = sel[1]
-        if start > end:
-            (start, end) = (end, start)
-            end_pos = sel[0]
-        if end > start and doc.GetColumn(end_pos) == 0:
-            end = end - 1
-        doc.BeginUndoAction()
-        for line in six.moves.range(start, end + 1):
-            firstChar = doc.PositionFromLine(line)
-            doc.InsertText(firstChar, text)
-        doc.SetCurrentPos(doc.PositionFromLine(start))
-        doc.SetAnchor(doc.GetLineEndPosition(end))
-        doc.EndUndoAction()
-        doc.Refresh()
-
-    def deprepandText(self, text):
-        """Uncomment section"""
-        doc = self
-        sel = doc.GetSelection()
-        start = doc.LineFromPosition(sel[0])
-        end = doc.LineFromPosition(sel[1])
-        end_pos = sel[1]
-        if start > end:
-            (start, end) = (end, start)
-            end_pos = sel[0]
-        if end > start and doc.GetColumn(end_pos) == 0:
-            end = end - 1
-        doc.BeginUndoAction()
-        for line in six.moves.range(start, end + 1):
-            firstChar = doc.PositionFromLine(line)
-            txt = doc.GetLine(line)
-            if txt.startswith(text):
-                doc.SetCurrentPos(firstChar + len(text))
-                doc.DelLineLeft()
-        doc.SetSelection(sel[0], doc.PositionFromLine(end + 1))
-        doc.SetCurrentPos(doc.PositionFromLine(start))
-        doc.EndUndoAction()
-        doc.Refresh()
-
-    def indented(self):
-        """increase the indent"""
-        tabWidth = max(1, self.GetTabWidth())
-        if self.GetUseTabs():
-            indentation = '\t'
-        else:
-            indentation = ' ' * tabWidth
-        self.prepandText(indentation)
-
-    def unindented(self):
-        """decrease the indent"""
-        tabWidth = max(1, self.GetTabWidth())
-        if self.GetUseTabs():
-            indentation = '\t'
-        else:
-            indentation = ' ' * tabWidth
-        self.deprepandText(indentation)
-
-    def comment(self):
-        """Comment section"""
-        self.prepandText('##')
-
-    def uncomment(self):
-        """Uncomment section"""
-        self.deprepandText('##')
-
-    def GetContextMenu(self):
-        """
-            Create and return a context menu for the shell.
-            This is used instead of the scintilla default menu
-            in order to correctly respect our immutable buffer.
-        """
-        menu = wx.Menu()
-        menu.Append(wx.ID_UNDO, 'Undo')
-        menu.Append(wx.ID_REDO, 'Redo')
-        menu.AppendSeparator()
-        menu.Append(wx.ID_CUT, 'Cut')
-        menu.Append(wx.ID_COPY, 'Copy')
-        menu.Append(wx.ID_PASTE, 'Paste')
-        menu.Append(wx.ID_CLEAR, 'Clear')
-        menu.AppendSeparator()
-        menu.Append(wx.ID_SELECTALL, 'Select All')
-        menu.AppendSeparator()
-        menu.Append(self.ID_COMMENT, 'Comment')
-        menu.Append(self.ID_UNCOMMENT, 'Uncomment')
-        return menu
-
-    def OnContextMenu(self, evt):
-        p = self.ScreenToClient(evt.GetPosition())
-        m = self.GetMarginWidth(0) + self.GetMarginWidth(1)
-        if p.x > m:
-            # show edit menu when the mouse is in editable area
-            menu = self.GetContextMenu()
-            self.PopupMenu(menu)
-        elif p.x > self.GetMarginWidth(0):
-            # in breakpoint area
-            cline = self.LineFromPosition(self.PositionFromPoint(p))
-            for key in self.breakpointlist:
-                line = self.MarkerLineFromHandle(key)
-                if line == cline:
-                    self.GotoLine(line)
-                    break
-            else:
-                return
-            menu = wx.Menu()
-            menu.Append(self.ID_DELETE_BREAKPOINT, 'Delete Breakpoint')
-            menu.AppendSeparator()
-            menu.Append(self.ID_EDIT_BREAKPOINT, 'Condition...')
-            menu.AppendSeparator()
-            menu.Append(self.ID_CLEAR_BREAKPOINT, 'Delete All Breakpoints')
-            self.PopupMenu(menu)
-
-    def OnUpdateCommandUI(self, evt):
-        eid = evt.Id
-        if eid in (wx.ID_CUT, wx.ID_CLEAR):
-            evt.Enable(self.GetSelectionStart() != self.GetSelectionEnd())
-        elif eid == wx.ID_COPY:
-            evt.Enable(self.GetSelectionStart() != self.GetSelectionEnd())
-        elif eid == wx.ID_PASTE:
-            evt.Enable(self.CanPaste())
-        elif eid == wx.ID_UNDO:
-            evt.Enable(self.CanUndo())
-        elif eid == wx.ID_REDO:
-            evt.Enable(self.CanRedo())
-        else:
-            evt.Skip()
-
-    def findBreakPoint(self, line):
-        for key in self.breakpointlist:
-            if line == self.MarkerLineFromHandle(key):
-                return self.breakpointlist[key]
-        return None
-
     def OnProcessEvent(self, evt):
         """process the menu command"""
         eid = evt.GetId()
-        if eid == wx.ID_CUT:
-            self.Cut()
-        elif eid == wx.ID_CLEAR:
-            self.ClearAll()
-        elif eid == wx.ID_COPY:
-            self.Copy()
-        elif eid == wx.ID_PASTE:
-            self.Paste()
-        elif eid == wx.ID_UNDO:
-            self.Undo()
-        elif eid == wx.ID_REDO:
-            self.Redo()
-        elif eid == wx.ID_SELECTALL:
-            self.SelectAll()
-        elif eid == self.ID_COMMENT:
+        super().OnProcessEvent(evt)
+
+        if eid == self.ID_COMMENT:
             self.comment()
         elif eid == self.ID_UNCOMMENT:
             self.uncomment()
         elif eid == self.ID_DELETE_BREAKPOINT:
             bp = self.findBreakPoint(self.GetCurrentLine())
             if bp:
                 dp.send('debugger.clear_breakpoint', id=bp['id'])
@@ -872,54 +441,61 @@
                 if dlg.ShowModal() == wx.ID_OK:
                     cond = dlg.GetCondition()
                     dp.send('debugger.edit_breakpoint',
                             id=bp['id'],
                             condition=cond[0],
                             hitcount=cond[1])
 
+    def LoadFile(self, filename):
+        """load file into editor"""
+        self.ClearBreakpoint()
+        if super().LoadFile(filename):
+            digits = np.max([np.ceil(np.log10(self.GetLineCount())), 1])
+            self.SetMarginWidth(0, int(25+digits*5))
+            return True
+        return False
 
 class PyEditorPanel(wx.Panel):
     Gce = Gcm()
     ID_RUN_SCRIPT = wx.NewId()
     ID_DEBUG_SCRIPT = wx.NewId()
-    ID_FIND_REPLACE = wx.NewId()
     ID_CHECK_SCRIPT = wx.NewId()
     ID_RUN_LINE = wx.NewId()
-    ID_FIND_NEXT = wx.NewId()
-    ID_FIND_PREV = wx.NewId()
+    ID_FIND_REPLACE = wx.NewId()
     ID_INDENT = wx.NewId()
     ID_UNINDENT = wx.NewId()
     ID_SETCURFOLDER = wx.NewId()
     ID_TIDY_SOURCE = wx.NewId()
     ID_SPLIT_VERT = wx.NewId()
     ID_SPLIT_HORZ = wx.NewId()
     ID_DBG_RUN = wx.NewId()
     ID_DBG_STOP = wx.NewId()
     ID_DBG_STEP = wx.NewId()
     ID_DBG_STEP_INTO = wx.NewId()
     ID_DBG_STEP_OUT = wx.NewId()
+    ID_PANE_COPY_PATH = wx.NewId()
+    ID_PANE_COPY_PATH_REL = wx.NewId()
+    ID_PANE_SHOW_IN_FINDER = wx.NewId()
+    ID_PANE_SHOW_IN_BROWSING = wx.NewId()
+    ID_PANE_CLOSE = wx.NewId()
+    ID_PANE_CLOSE_OTHERS = wx.NewId()
+    ID_PANE_CLOSE_ALL = wx.NewId()
+
     wildcard = 'Python source (*.py)|*.py|Text (*.txt)|*.txt|All files (*.*)|*.*'
     frame = None
 
     def __init__(self, parent):
         wx.Panel.__init__(self, parent, size=(1, 1))
-        # find & replace dialog
-        self.findStr = ""
-        self.replaceStr = ""
-        self.findFlags = 1
-        self.stcFindFlags = 0
-        self.wrapped = 0
 
         self.fileName = """"""
         self.splitter = wx.SplitterWindow(self, style=wx.SP_LIVE_UPDATE)
         self.editor = PyEditor(self.splitter)
         self.editor2 = None
         self.splitter.Initialize(self.editor)
         self.Bind(stc.EVT_STC_CHANGE, self.OnCodeModified)
-        self.findDialog = None
         item = (
             (wx.ID_OPEN, 'Open', open_xpm, 'Open Python script'),
             (wx.ID_REFRESH, 'Reload', reload_xpm, 'Reload current script'),
             (wx.ID_SAVE, 'Save', save_xpm, 'Save current document (Ctrl+S)'),
             (wx.ID_SAVEAS, 'Save As', saveas_xpm, 'Save current document as'),
             (None, None, None, None),
             (self.ID_FIND_REPLACE, 'Find', find_xpm, 'Find/Replace (Ctrl+F)'),
@@ -943,19 +519,17 @@
             (self.ID_SPLIT_VERT, 'Split Vert', vert_xpm,
              'Split the window vertically'),
             (self.ID_SPLIT_HORZ, 'Split Horz', horz_xpm,
              'Split the window horizontally'),
         )
 
         self.toolbarart = AuiToolBarPopupArt(self)
-        self.tb = aui.AuiToolBar(self,
-                                 agwStyle=aui.AUI_TB_OVERFLOW
-                                 | aui.AUI_TB_PLAIN_BACKGROUND)
+        self.tb = aui.AuiToolBar(self, agwStyle=aui.AUI_TB_OVERFLOW)
         for (eid, label, img_xpm, tooltip) in item:
-            if eid == None:
+            if eid is None:
                 self.tb.AddSeparator()
                 continue
             bmp = wx.Bitmap(to_byte(img_xpm))
             if label in ['Split Vert', 'Split Horz']:
                 self.tb.AddCheckTool(eid, label, bmp, wx.NullBitmap, tooltip)
             else:
                 self.tb.AddSimpleTool(eid, label, bmp, tooltip)
@@ -964,15 +538,15 @@
         self.cbWrapMode.SetValue(True)
         self.tb.AddControl(self.cbWrapMode)
 
         self.tb.SetArtProvider(self.toolbarart)
         self.tb.Realize()
         self.box = wx.BoxSizer(wx.VERTICAL)
         self.box.Add(self.tb, 0, wx.EXPAND, 5)
-        self.box.Add(wx.StaticLine(self), 0, wx.EXPAND)
+        #self.box.Add(wx.StaticLine(self), 0, wx.EXPAND)
         self.box.Add(self.splitter, 1, wx.EXPAND)
         self.box.Fit(self)
         self.SetSizer(self.box)
         # Connect Events
         self.Bind(wx.EVT_TOOL, self.OnBtnOpen, id=wx.ID_OPEN)
         self.Bind(wx.EVT_TOOL, self.OnBtnReload, id=wx.ID_REFRESH)
         self.Bind(wx.EVT_TOOL, self.OnBtnSave, id=wx.ID_SAVE)
@@ -980,27 +554,21 @@
         self.tb.Bind(wx.EVT_UPDATE_UI, self.OnUpdateBtn)
         self.Bind(wx.EVT_TOOL, self.OnShowFindReplace, id=self.ID_FIND_REPLACE)
         self.Bind(wx.EVT_TOOL, self.OnBtnRun, id=self.ID_RUN_LINE)
         self.Bind(wx.EVT_TOOL, self.OnBtnCheck, id=self.ID_CHECK_SCRIPT)
         self.Bind(wx.EVT_TOOL, self.OnBtnRunScript, id=self.ID_RUN_SCRIPT)
         self.Bind(wx.EVT_TOOL, self.OnBtnDebugScript, id=self.ID_DEBUG_SCRIPT)
         #self.Bind(wx.EVT_UPDATE_UI, self.OnUpdateBtn, id=self.ID_DEBUG_SCRIPT)
-        self.Bind(wx.EVT_TOOL, self.OnFindNext, id=self.ID_FIND_NEXT)
-        self.Bind(wx.EVT_TOOL, self.OnFindPrev, id=self.ID_FIND_PREV)
         self.Bind(wx.EVT_TOOL, self.OnIndent, id=self.ID_INDENT)
         self.Bind(wx.EVT_TOOL, self.OnUnindent, id=self.ID_UNINDENT)
         self.Bind(wx.EVT_TOOL, self.OnSetCurFolder, id=self.ID_SETCURFOLDER)
         self.Bind(wx.EVT_TOOL, self.OnSplitVert, id=self.ID_SPLIT_VERT)
         self.Bind(wx.EVT_TOOL, self.OnSplitHorz, id=self.ID_SPLIT_HORZ)
         self.cbWrapMode.Bind(wx.EVT_CHECKBOX, self.OnWrap)
         accel = [
-            (wx.ACCEL_CTRL, ord('F'), self.ID_FIND_REPLACE),
-            (wx.ACCEL_NORMAL, wx.WXK_F3, self.ID_FIND_NEXT),
-            (wx.ACCEL_SHIFT, wx.WXK_F3, self.ID_FIND_PREV),
-            (wx.ACCEL_CTRL, ord('H'), self.ID_FIND_REPLACE),
             (wx.ACCEL_CTRL, wx.WXK_RETURN, self.ID_RUN_LINE),
             (wx.ACCEL_CTRL, ord('S'), wx.ID_SAVE),
         ]
         self.accel = wx.AcceleratorTable(accel)
         self.SetAcceleratorTable(self.accel)
         #dp.connect(self.debug_paused, 'debugger.paused')
         dp.connect(self.debug_ended, 'debugger.ended')
@@ -1016,15 +584,15 @@
             yield inst
 
     def Destroy(self):
         """destroy the panel"""
         self.editor.ClearBreakpoint()
         self.CheckModified()
         self.Gce.destroy(self.num)
-        return super(PyEditorPanel, self).Destroy()
+        return super().Destroy()
 
     def update_bp(self):
         """update the breakpoints"""
         for key in self.editor.breakpointlist:
             line = self.editor.MarkerLineFromHandle(key) + 1
             if line != self.editor.breakpointlist[key]['lineno']:
                 ids = self.editor.breakpointlist[key]['id']
@@ -1038,15 +606,15 @@
         filename = info['filename']
         if filename != self.editor.filename:
             return
         for key in self.editor.breakpointlist:
             if self.editor.breakpointlist[key]['id'] == bpdata['id']:
                 return
         lineno = info['lineno']
-        handler = self.editor.MarkerAdd(lineno - 1, 0)
+        handler = self.editor.MarkerAdd(lineno - 1, MARKER_BP)
         self.editor.breakpointlist[handler] = bpdata
 
     def debug_bpcleared(self, bpdata):
         """the breakpoint is cleared"""
         if bpdata is None:
             return
         info = bpdata
@@ -1070,25 +638,24 @@
         filename = status['filename']
 
         lineno = -1
         marker = -1
         active = False
         if filename == self.editor.filename:
             lineno = status['lineno']
-            marker = 1
+            marker = MARKER_BP_PAUSED_CUR
             active = True
         else:
             frames = status['frames']
             if frames is not None:
                 for frame in frames:
-                    filename = inspect.getsourcefile(frame) or inspect.getfile(
-                        frame)
+                    filename = frame.f_code.co_filename
                     if filename == self.fileName:
                         lineno = frame.f_lineno
-                        marker = 2
+                        marker = MARKER_BP_PAUSED
                         break
         if lineno >= 0 and marker >= 0:
             self.debug_curline = self.editor.MarkerAdd(lineno - 1, marker)
             self.editor.EnsureVisibleEnforcePolicy(lineno - 1)
             #self.JumpToLine(lineno-1)
             #self.editor.GotoLine(lineno-1)
             #self.editor.EnsureVisible(lineno-1)
@@ -1215,58 +782,32 @@
                 event.Enable(not resp[0][1])
         elif eid == wx.ID_REFRESH:
             event.Enable(self.fileName != "")
 
     def OnShowFindReplace(self, event):
         """Find and Replace dialog and action."""
         # find string
-        findStr = self.editor.GetSelectedText()
-        if findStr and self.findDialog:
-            self.findDialog.Destroy()
-            self.findDialog = None
-        # dialog already open, if yes give focus
-        if self.findDialog:
-            self.findDialog.Show(1)
-            self.findDialog.Raise()
-            return
-        if not findStr:
-            findStr = self.findStr
-        # find data
-        data = wx.FindReplaceData(self.findFlags)
-        data.SetFindString(findStr)
-        data.SetReplaceString(self.replaceStr)
-        # dialog
-        self.findDialog = wx.FindReplaceDialog(
-            self, data, 'Find & Replace', wx.FR_REPLACEDIALOG)
-        # bind the event to the dialog, see the example in wxPython demo
-        self.findDialog.Bind(wx.EVT_FIND, self.OnFind)
-        self.findDialog.Bind(wx.EVT_FIND_NEXT, self.OnFind)
-        self.findDialog.Bind(wx.EVT_FIND_REPLACE, self.OnReplace)
-        self.findDialog.Bind(wx.EVT_FIND_REPLACE_ALL, self.OnReplaceAll)
-        self.findDialog.Bind(wx.EVT_FIND_CLOSE, self.OnFindClose)
-        self.findDialog.Show(1)
-        self.findDialog.data = data  # save a reference to it...
+        self.editor.OnShowFindReplace(event)
 
     def RunCommand(self, command, prompt=False, verbose=True, debug=False):
         """run command in shell"""
         dp.send('shell.run',
                 command=command,
                 prompt=prompt,
                 verbose=verbose,
-                debug=debug)
+                debug=debug,
+                history=False)
 
     def OnBtnRun(self, event):
         """execute the selection or current line"""
         cmd = self.editor.GetSelectedText()
         if not cmd or cmd == """""":
             (cmd, _) = self.editor.GetCurLine()
             cmd = cmd.rstrip()
-        lines = cmd.split('\n')
-        for line in lines:
-            self.RunCommand(line, prompt=True, verbose=True)
+        self.RunCommand(cmd, prompt=True, verbose=True)
 
     def CheckModified(self):
         """check whether it is modified"""
         if self.editor.GetModify():
             msg = 'The file has been modified. Save it first?'
             # use top level frame as parent, otherwise it may crash when
             # it is called in Destroy()
@@ -1285,18 +826,18 @@
             return
         if self.fileName == """""":
             return
         self.RunCommand('import sys', verbose=False)
         self.RunCommand('_bsm_source = open(r\'%s\',\'r\').read()+\'\\n\'' %
                         self.fileName,
                         verbose=False)
-        self.RunCommand('compile(_bsm_source,r\'%s\',\'exec\')' %
+        self.RunCommand('_bsm_code = compile(_bsm_source,r\'%s\',\'exec\')' %
                         self.fileName,
                         prompt=True,
-                        verbose=True)
+                        verbose=False)
         self.RunCommand('del _bsm_source', verbose=False)
 
     def OnBtnRunScript(self, event):
         """execute the script"""
         if self.CheckModified():
             return
         if not self.fileName:
@@ -1325,141 +866,34 @@
                         prompt=True,
                         verbose=False,
                         debug=True)
 
         #dp.send('debugger.ended')
         self.tb.EnableTool(self.ID_DEBUG_SCRIPT, True)
 
-    def message(self, text):
-        """show the message on statusbar"""
-        dp.send('frame.show_status_text', text=text)
-
-    def _find_text(self, minPos, maxPos, text, flags=0):
-        position = self.editor.FindText(minPos, maxPos, text, flags)
-        if isinstance(position, tuple):
-            position = position[0] # wx ver 4.1.0 returns (start, end)
-        return position
-
-    def doFind(self, strFind, forward=True):
-        """search the string"""
-        current = self.editor.GetCurrentPos()
-        position = -1
-        if forward:
-            position = self._find_text(current, len(self.editor.GetText()),
-                                       strFind, self.stcFindFlags)
-            if position == -1:
-                # wrap around
-                self.wrapped += 1
-                position = self._find_text(0, current + len(strFind), strFind,
-                                           self.stcFindFlags)
-        else:
-            position = self._find_text(current - len(strFind), 0, strFind,
-                                       self.stcFindFlags)
-            if position == -1:
-                # wrap around
-                self.wrapped += 1
-                position = self._find_text(len(self.editor.GetText()), current,
-                                           strFind, self.stcFindFlags)
-
-        # not found the target, do not change the current position
-        if position == -1:
-            self.message("'%s' not found!" % strFind)
-            position = current
-            strFind = """"""
-        self.editor.GotoPos(position)
-        self.editor.SetSelection(position, position + len(strFind))
-        return position
-
-    def OnFind(self, event):
-        """search the string"""
-        self.findStr = event.GetFindString()
-        self.findFlags = event.GetFlags()
-        flags = 0
-        if wx.FR_WHOLEWORD & self.findFlags:
-            flags |= stc.STC_FIND_WHOLEWORD
-        if wx.FR_MATCHCASE & self.findFlags:
-            flags |= stc.STC_FIND_MATCHCASE
-        self.stcFindFlags = flags
-        return self.doFind(self.findStr, wx.FR_DOWN & self.findFlags)
-
-    def OnFindClose(self, event):
-        """close find & replace dialog"""
-        event.GetDialog().Destroy()
-
-    def OnReplace(self, event):
-        """replace"""
-        # Next line avoid infinite loop
-        findStr = event.GetFindString()
-        self.replaceStr = event.GetReplaceString()
-
-        source = self.editor
-        selection = source.GetSelectedText()
-        if not event.GetFlags() & wx.FR_MATCHCASE:
-            findStr = findStr.lower()
-            selection = selection.lower()
-
-        if selection == findStr:
-            position = source.GetSelectionStart()
-            source.ReplaceSelection(self.replaceStr)
-            source.SetSelection(position, position + len(self.replaceStr))
-        # jump to next instance
-        position = self.OnFind(event)
-        return position
-
-    def OnReplaceAll(self, event):
-        """replace all the instances"""
-        source = self.editor
-        count = 0
-        self.wrapped = 0
-        position = start = source.GetCurrentPos()
-        while position > -1 and (not self.wrapped or position < start):
-            position = self.OnReplace(event)
-            if position != -1:
-                count += 1
-            if self.wrapped >= 2:
-                break
-        self.editor.GotoPos(start)
-        if not count:
-            self.message("'%s' not found!" % event.GetFindString())
-
-    def OnFindNext(self, event):
-        """go the previous instance of search string"""
-        findStr = self.editor.GetSelectedText()
-        if findStr:
-            self.findStr = findStr
-        if self.findStr:
-            self.doFind(self.findStr)
-
-    def OnFindPrev(self, event):
-        """go the previous instance of search string"""
-        findStr = self.editor.GetSelectedText()
-        if findStr:
-            self.findStr = findStr
-        if self.findStr:
-            self.doFind(self.findStr, False)
 
     def OnIndent(self, event):
         """increase the indent"""
         self.editor.indented()
 
     def OnUnindent(self, event):
         """decrease the indent"""
         self.editor.unindented()
 
     def OnSetCurFolder(self, event):
         """set the current folder to the folder with the file"""
         if not self.fileName:
             return
-        path, = os.path.split(self.fileName)
+        path, _ = os.path.split(self.fileName)
         self.RunCommand('import os', verbose=False)
         self.RunCommand('os.chdir(r\'%s\')' % path, verbose=False)
 
     def OnSplitVert(self, event):
         """show splitter window vertically"""
-        show = self.tb.GetToolState(self.ID_SPLIT_VERT)
+        show = self.tb.GetToolToggled(self.ID_SPLIT_VERT)
         if not show:
             # hide the splitter window
             if self.editor2:
                 if self.splitter.IsSplit():
                     self.splitter.Unsplit(self.editor2)
                 self.editor2.Hide()
         else:
@@ -1472,15 +906,15 @@
                 if self.splitter.IsSplit():
                     self.splitter.Unsplit(self.editor2)
                 self.splitter.SplitHorizontally(self.editor, self.editor2)
                 self.tb.ToggleTool(self.ID_SPLIT_HORZ, False)
 
     def OnSplitHorz(self, event):
         """show splitter window horizontally"""
-        show = self.tb.GetToolState(self.ID_SPLIT_HORZ)
+        show = self.tb.GetToolToggled(self.ID_SPLIT_HORZ)
         if not show:
             # hide the splitter window
             if self.editor2:
                 if self.splitter.IsSplit():
                     self.splitter.Unsplit(self.editor2)
                 self.editor2.Hide()
         else:
@@ -1510,18 +944,57 @@
             cls.ID_EDITOR_NEW = resp[0][1]
         resp = dp.send('frame.add_menu',
                        path='File:Open:Python script\tCtrl+O',
                        rxsignal='bsm.editor.menu')
         if resp:
             cls.ID_EDITOR_OPEN = resp[0][1]
         dp.connect(cls.ProcessCommand, 'bsm.editor.menu')
+        dp.connect(cls.PaneMenu, 'bsm.editor.pane_menu')
         dp.connect(cls.Uninitialize, 'frame.exit')
+        dp.connect(cls.OnFrameClosing, 'frame.closing')
         dp.connect(cls.OpenScript, 'frame.file_drop')
         dp.connect(cls.DebugPaused, 'debugger.paused')
         dp.connect(cls.DebugUpdateScope, 'debugger.update_scopes')
+        dp.connect(cls.SetActive, 'frame.activate_panel')
+        dp.connect(receiver=cls.Initialized, signal='frame.initialized')
+
+
+    @classmethod
+    def PaneMenu(cls, pane, command):
+        if not pane or not isinstance(pane, PyEditorPanel):
+            return
+        if command in [cls.ID_PANE_COPY_PATH, cls.ID_PANE_COPY_PATH_REL]:
+            if wx.TheClipboard.Open():
+                filepath = pane.fileName
+                if command == cls.ID_PANE_COPY_PATH_REL:
+                    filepath = os.path.relpath(filepath, os.getcwd())
+                wx.TheClipboard.SetData(wx.TextDataObject(filepath))
+                wx.TheClipboard.Close()
+        elif command == cls.ID_PANE_SHOW_IN_FINDER:
+            show_file_in_finder(pane.fileName)
+        elif command == cls.ID_PANE_SHOW_IN_BROWSING:
+            dp.send(signal='dirpanel.goto', filepath=pane.fileName, show=True)
+        elif command == cls.ID_PANE_CLOSE:
+            dp.send(signal='frame.delete_panel', panel=pane)
+        elif command == cls.ID_PANE_CLOSE_OTHERS:
+            mgrs =  PyEditorPanel.Gce.get_all_managers()
+            for mgr in mgrs:
+                if mgr == pane:
+                    continue
+                dp.send(signal='frame.delete_panel', panel=mgr)
+        elif command == cls.ID_PANE_CLOSE_ALL:
+            mgrs =  PyEditorPanel.Gce.get_all_managers()
+            for mgr in mgrs:
+                dp.send(signal='frame.delete_panel', panel=mgr)
+
+    @classmethod
+    def SetActive(cls, pane):
+        """set the active figure"""
+        if pane and isinstance(pane, PyEditorPanel):
+            cls.Gce.set_active(pane)
 
     @classmethod
     def DebugPaused(cls):
         """the debugger has paused, update the editor margin marker"""
         resp = dp.send('debugger.get_status')
         if not resp or not resp[0][1]:
             return
@@ -1544,17 +1017,47 @@
         if not resp or not resp[0][1]:
             return
         status = resp[0][1]
         for editor in PyEditorPanel.get_instances():
             editor.debug_paused(status)
 
     @classmethod
+    def Initialized(cls):
+        resp = dp.send('frame.get_config', group='editor', key='opened')
+        if resp and resp[0][1]:
+            files = resp[0][1]
+            if len(files[0]) == 2:
+                files = [ f+[False] for f in files]
+            for f, line, shown in files:
+                cls.OpenScript(f, activated=False, lineno=line)
+
+            for f, line, shown in files:
+                if shown:
+                    wx.CallAfter(cls.OpenScript, filename=f, activated=True, lineno=line)
+
+    @classmethod
+    def OnFrameClosing(cls, event):
+        """the frame is exiting"""
+        for panel in cls.Gce.get_all_managers():
+            if panel.CheckModified():
+                # the file has been modified, stop closing
+                event.Veto()
+                break
+
+    @classmethod
     def Uninitialize(cls):
         """unload the module"""
-        pass
+        files = []
+        for panel in cls.Gce.get_all_managers():
+            editor = panel.editor
+            files.append([editor.filename, editor.GetCurrentLine(), panel.IsShown()])
+
+        for panel in cls.Gce.get_all_managers():
+            dp.send('frame.delete_panel', panel=panel)
+        dp.send('frame.set_config', group='editor', opened=files)
 
     @classmethod
     def ProcessCommand(cls, command):
         """process the menu command"""
         if command == cls.ID_EDITOR_NEW:
             cls.AddEditor()
         elif command == cls.ID_EDITOR_OPEN:
@@ -1577,15 +1080,27 @@
         editor = PyEditorPanel(cls.frame)
 
         direction = cls.kwargs.get('direction', 'top')
         dp.send("frame.add_panel",
                 panel=editor,
                 title=title,
                 active=activated,
-                direction=direction)
+                direction=direction,
+                pane_menu={'rxsignal': 'bsm.editor.pane_menu',
+                           'menu': [
+                               {'id':cls.ID_PANE_CLOSE, 'label':'Close\tCtrl+W'},
+                               {'id':cls.ID_PANE_CLOSE_OTHERS, 'label':'Close Others'},
+                               {'id':cls.ID_PANE_CLOSE_ALL, 'label':'Close All'},
+                               {'type': wx.ITEM_SEPARATOR},
+                               {'id':cls.ID_PANE_COPY_PATH, 'label':'Copy Path\tAlt+Ctrl+C'},
+                               {'id':cls.ID_PANE_COPY_PATH_REL, 'label':'Copy Relative Path\tAlt+Shift+Ctrl+C'},
+                               {'type': wx.ITEM_SEPARATOR},
+                               {'id': cls.ID_PANE_SHOW_IN_FINDER, 'label':f'Reveal in  {get_file_finder_name()}\tAlt+Ctrl+R'},
+                               {'id': cls.ID_PANE_SHOW_IN_BROWSING, 'label':'Reveal in Browsing panel'},
+                               ]})
         return editor
 
     @classmethod
     def OpenScript(cls, filename, activated=True, lineno=0):
         """open the file"""
         if not filename:
             return None
@@ -1598,15 +1113,15 @@
             editor = cls.AddEditor()
             editor.LoadFile(filename)
             dp.send('frame.add_file_history', filename=filename)
 
         if editor and activated and not editor.IsShown():
             dp.send('frame.show_panel', panel=editor, focus=True)
         if lineno > 0:
-            editor.JumpToLine(lineno - 1, True)
+            editor.JumpToLine(lineno - 1)
         return editor
 
     @classmethod
     def findEditorByFileName(cls, filename):
         """
         find the editor by filename
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/graph.py` & `bsmedit-3.2.9/bsmedit/bsm/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,262 +1,109 @@
-import math
 import wx
-import wx.aui
 import wx.py.dispatcher as dp
-import numpy
+import numpy as np
 import matplotlib
 matplotlib.use('module://bsmedit.bsm.bsmbackend')
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas
 from matplotlib.backends.backend_wx import NavigationToolbar2Wx as NavigationToolbar
 from matplotlib.backends.backend_wx import FigureManagerWx
 from matplotlib._pylab_helpers import Gcf
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
+from .graph_common import GraphObject
 from .lineeditor import LineEditor
-from .utility import PopupMenu
+from .graph_datatip import DataCursor
+from .utility import PopupMenu, build_menu_from_list, svg_to_bitmap
 from .bsmxpm import home_xpm, back_xpm, forward_xpm, pan_xpm, zoom_xpm, \
-                    cursor_xpm, save_xpm, copy_xpm, line_edit_xpm, page_add_xpm
+                    cursor_xpm, save_xpm, copy_xpm, line_edit_xpm, page_add_xpm, \
+                    more_svg
 from .. import to_byte
+from .graph_toolbar import GraphToolbar
 rcParams.update({'figure.autolayout': True})
 rcParams.update({'toolbar': 'None'})
 matplotlib.interactive(True)
 
 
-class DataCursor(object):
-    xoffset, yoffset = -20, 20
-    text_template = 'x: %0.2f\ny: %0.2f'
-
-    ID_DELETE_DATATIP = wx.NewId()
-    ID_CLEAR_DATATIP = wx.NewId()
-    def __init__(self):
-        self.annotations = []
-        self.lines = []
-        self.enable = False
-        self.active = None
-        self.mx, self.my = None, None
-        self.pickEvent = False
-
-    def pick(self, event):
-        if not self.enable:
-            return
-        if not event.mouseevent.xdata or not event.mouseevent.ydata:
-            return
-        if not event.artist:
-            return
-        xm, ym = event.mouseevent.x, event.mouseevent.y
-        if self.get_annotation(xm, ym) is not None:
-            # click in the box of existing annotation, ignore it
-            return
-
-        line = event.artist
-        if self.active and self.active.get_visible():
-            # Check whether the axes of active annotation is same as line,
-            # which may happen in a figure with subplots. If not, create one
-            # with the axes of line
-            if self.active.axes != line.axes:
-                self.active = None
-        if self.active is None:
-            self.create_annotation(line)
-        idx = self.annotations.index(self.active)
-        self.lines[idx] = line
-
-        # find the closest point on the line
-        x, y = line.get_xdata(), line.get_ydata()
-        xc, yc = event.mouseevent.xdata, event.mouseevent.ydata
-        idx = (numpy.square(x - xc) + numpy.square(y - yc)).argmin()
-        xn, yn = x[idx], y[idx]
-        if xn is not None:
-            self.active.xy = xn, yn
-            self.active.set_text(self.text_template % (xn, yn))
-            self.active.set_visible(True)
-            event.canvas.draw()
-        self.pickEvent = True
-
-    def keyboard_move(self, left, step=1):
-        if not self.active:
-            return
-        idx = self.annotations.index(self.active)
-        line = self.lines[idx]
-        x, y = line.get_xdata(), line.get_ydata()
-        xc, yc = self.active.xy
-        idx = (numpy.square(x - xc)).argmin()
-        idx_new = idx
-        if left:
-            idx_new -= step
-        else:
-            idx_new += step
-        idx_new = min(len(x)-1, idx_new)
-        idx_new = max(0, idx_new)
-        if idx == idx_new:
-            return
-        xn, yn = x[idx_new], y[idx_new]
-        if xn is not None:
-            self.active.xy = xn, yn
-            self.active.set_text(self.text_template % (xn, yn))
-            self.active.set_visible(True)
-
-    def set_enable(self, enable):
-        self.enable = enable
-        if self.active:
-            if enable:
-                self.active.get_bbox_patch().set_facecolor('yellow')
-            else:
-                self.active.get_bbox_patch().set_facecolor('white')
+class Pan(GraphObject):
+    def __init__(self, figure):
+        super().__init__(figure)
+        self.axes = None
+
+    def key_down(self, event):
+        keycode = event.GetKeyCode()
+        axes = self.axes
+        if axes is None:
+            if len(self.figure.get_axes()) > 1:
+                return
+            axes = [self.figure.gca()]
+        xlims_all = []
+        ylims_all = []
+        for ax in axes:
+            # get the xlim from all axes first, as some x-axis may be shared;
+            # otherwise, the shared x-axis will be moved multiple times.
+            xlims_all.append(np.array(ax.get_xlim()))
+            ylims_all.append(np.array(ax.get_ylim()))
+        step = 1
+        if event.ShiftDown():
+            step = 1/10
+        for i, ax in enumerate(axes):
+            xlims = xlims_all[i]
+            ylims = ylims_all[i]
+            rng_x = (xlims[1] - xlims[0])*step
+            rng_y = (ylims[1] - ylims[0])*step
+            if keycode in [wx.WXK_LEFT, wx.WXK_RIGHT]:
+                if keycode == wx.WXK_LEFT:
+                    xlims -= rng_x
+                else:
+                    xlims += rng_x
 
-    def mouse_move(self, event):
-        """move the annotation position"""
-        # return if no active annotation or the mouse is not pressed
-        if self.mx is None or self.my is None or self.active is None:
-            return False
-        # re-position the active annotation based on the mouse movement
-        x, y = event.x, event.y
-        dx = x - self.mx
-        dy = y - self.my
-        dis = math.sqrt(dx**2 + dy**2)
-        if dis > 50:
-            (px, py) = (-20, 20)
-            if dx > 80:
-                px = 60
-            elif dx > 40:
-                px = 20
-            if dy < -80:
-                py = -60
-            elif dy < -40:
-                py = -20
-            self.active.xyann = (px, py)
-            return True
-        return False
+                ax.set_xlim(xlims)
+                # rescale y to show data
+                #ax.autoscale(axis='y')
+            elif keycode in [wx.WXK_UP, wx.WXK_DOWN]:
+                if keycode == wx.WXK_UP:
+                    ylims += rng_y
+                else:
+                    ylims -= rng_y
 
-    def get_annotation(self, x, y):
-        for ant in self.annotations:
-            box = ant.get_bbox_patch().get_extents()
-            if box.contains(x, y):
-                return ant
-        return None
+                ax.set_ylim(ylims)
+                #ax.autoscale(axis='x')
+            else:
+                event.Skip()
+        self.figure.canvas.draw_idle()
 
     def mouse_pressed(self, event):
-        """
-        select the active annotation which is closest to the mouse position
-        """
-        # ignore the event triggered immediately after pick_event
-        if self.pickEvent:
-            self.pickEvent = False
-            return False
-        # just created the new annotation, do not move to others
-        if self.active and (not self.active.get_visible()):
-            return False
-        # search the closest annotation
-        x, y = event.x, event.y
-        self.mx, self.my = x, y
-        active = self.get_annotation(x, y)
-        self.set_active(active)
-        # return True for the parent to redraw
-        return True
-
-    def mouse_released(self, event):
-        """release the mouse"""
-        self.mx, self.my = None, None
-
-    def get_active(self):
-        """retrieve the active annotation"""
-        return self.active
-
-    def set_active(self, ant):
-        """set the active annotation"""
-        if ant and (ant not in self.annotations):
-            return False
-        if self.active == ant:
-            return True
-        if self.active:
-            self.active.get_bbox_patch().set_facecolor('white')
-        self.active = ant
-        if self.active:
-            self.active.get_bbox_patch().set_facecolor('yellow')
-        return True
-
-    def get_annotations(self):
-        """return all the annotations"""
-        return self.annotations
-
-    def create_annotation(self, line):
-        """create the annotation and set it active"""
-        ant = line.axes.annotate(self.text_template,
-                                 xy=(0, 0),
-                                 xytext=(self.xoffset, self.yoffset),
-                                 textcoords='offset points',
-                                 ha='right',
-                                 va='bottom',
-                                 bbox=dict(boxstyle='round,pad=0.5',
-                                           fc='yellow',
-                                           alpha=0.5),
-                                 arrowprops=dict(arrowstyle='->',
-                                                 connectionstyle='arc3,rad=0'))
-        ant.set_visible(False)
-        self.annotations.append(ant)
-        self.lines.append(line)
-        self.set_active(ant)
-
-    def GetMenu(self):
-        cmd = [[self.ID_DELETE_DATATIP, 'Delete current datatip',
-                self.active is not None and self.active.get_visible()],
-               [self.ID_CLEAR_DATATIP, 'Delete all datatip', len(self.annotations) > 0]
-              ]
-        return cmd
-
-    def ProcessCommand(self, cmd):
-        """process the context menu command"""
-        if cmd == self.ID_DELETE_DATATIP:
-            if not self.active:
-                return False
-            idx = self.annotations.index(self.active)
-            self.active.remove()
-            del self.annotations[idx]
-            del self.lines[idx]
-            self.active = None
-            return True
-        elif cmd == self.ID_CLEAR_DATATIP:
-            for ant in self.annotations:
-                try:
-                    # the call may fail. For example,
-                    # 1) create a figure and plot some curve
-                    # 2) create a datatip
-                    # 3) call clf() to clear the figure, the datatip will be
-                    #    cleared, but we will not know
-                    ant.remove()
-                except:
-                    pass
-            self.annotations = []
-            self.lines = []
-            self.active = None
-            return True
+        self.axes = [a for a in self.figure.get_axes()
+                if a.in_axes(event)]
         return False
 
-    def activated(self):
-        pass
-    def deactivated(self):
-        pass
+class Toolbar(GraphToolbar):
+    ID_AUTO_SCALE_X = wx.NewId()
+    ID_AUTO_SCALE_Y = wx.NewId()
+    ID_AUTO_SCALE_XY = wx.NewId()
 
-class Toolbar(NavigationToolbar):
     def __init__(self, canvas, figure):
         if matplotlib.__version__ < '3.3.0':
             self._init_toolbar = self.init_toolbar
         else:
             self._init_toolbar = self.init_toolbar_empty
-        NavigationToolbar.__init__(self, canvas)
+        GraphToolbar.__init__(self, canvas)
 
         if matplotlib.__version__ >= '3.3.0':
             self.init_toolbar()
         self.SetWindowStyle(wx.TB_HORIZONTAL | wx.TB_FLAT)
         self.figure = figure
-        self.datacursor = DataCursor()
+        self.datacursor = DataCursor(self.figure, self)
         self.lineeditor = LineEditor(self.figure)
+        self.pan_action = Pan(self.figure)
 
         self.actions = {'datatip': self.datacursor,
-                        'edit': self.lineeditor}
+                        'edit': self.lineeditor,
+                        'pan/zoom': self.pan_action}
 
         self.canvas.mpl_connect('pick_event', self.OnPick)
         self.canvas.mpl_connect('motion_notify_event', self.OnMove)
         self.canvas.mpl_connect('button_press_event', self.OnPressed)
         self.canvas.mpl_connect('button_release_event', self.OnReleased)
         self.canvas.mpl_connect('scroll_event', self.OnZoomFun)
         self.canvas.mpl_connect('key_press_event', self.OnKeyPressed)
@@ -265,14 +112,20 @@
 
     def GetMenu(self):
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'GetMenu'):
             return []
         return action.GetMenu()
 
+    def key_down(self, event):
+        action = self.actions.get(self.mode, None)
+        if action is None or not hasattr(action, 'key_down'):
+            return
+        action.key_down(event)
+
     def ProcessCommand(self, cmd):
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'ProcessCommand'):
             return
         action.ProcessCommand(cmd)
 
     def OnPick(self, event):
@@ -283,21 +136,26 @@
 
     def OnKeyPressed(self, event):
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'key_pressed'):
             return
         action.key_pressed(event)
 
+    def _set_picker_all(self):
+        for g in self.figure.get_axes():
+            for l in g.lines:
+                if l.get_picker() is None:
+                    l.set_picker(5)
+
     def OnPressed(self, event):
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'mouse_pressed'):
             return
         # some lines may be added
-        for l in self.figure.gca().lines:
-            l.set_picker(5)
+        self._set_picker_all()
         if action.mouse_pressed(event):
             self.canvas.draw()
 
     def OnReleased(self, event):
         action = self.actions.get(self.mode, None)
         if action is None or not hasattr(action, 'mouse_released'):
             return
@@ -308,22 +166,25 @@
         if action is None or not hasattr(action, 'mouse_move'):
             return
         if action.mouse_move(event):
             self.canvas.draw()
 
     def OnZoomFun(self, event):
         # get the current x and y limits
-        if not self.GetToolState(self.wx_ids['Zoom']):
+        if not self.GetToolToggled(self.wx_ids['Zoom']):
             return
         if self._nav_stack.empty():
             self.push_current()
+
+        axes = [a for a in self.figure.get_axes()
+                if a.in_axes(event)]
+        if not axes:
+            return
+
         base_scale = 2.0
-        ax = self.figure.gca()
-        cur_xlim = ax.get_xlim()
-        cur_ylim = ax.get_ylim()
 
         xdata = event.xdata  # get event x location
         ydata = event.ydata  # get event y location
         if xdata is None:
             return
         if ydata is None:
             return
@@ -334,30 +195,33 @@
         elif event.button == 'up':
             # deal with zoom out
             scale_factor = base_scale
         else:
             # deal with something that should never happen
             scale_factor = 1.0
 
-        new_width = (cur_xlim[1] - cur_xlim[0]) * scale_factor
-        new_height = (cur_ylim[1] - cur_ylim[0]) * scale_factor
-
-        relx = (cur_xlim[1] - xdata) / (cur_xlim[1] - cur_xlim[0])
-        rely = (cur_ylim[1] - ydata) / (cur_ylim[1] - cur_ylim[0])
-        xzoom = yzoom = True
-        if wx.GetKeyState(wx.WXK_CONTROL_X):
-            yzoom = False
-        elif wx.GetKeyState(wx.WXK_CONTROL_Y):
-            xzoom = False
-        if (xzoom) and new_width * (1 - relx) > 0:
-            ax.set_xlim(
-                [xdata - new_width * (1 - relx), xdata + new_width * (relx)])
-        if (yzoom) and new_height * (1 - rely) > 0:
-            ax.set_ylim(
-                [ydata - new_height * (1 - rely), ydata + new_height * (rely)])
+        for ax in axes:
+            cur_xlim = ax.get_xlim()
+            cur_ylim = ax.get_ylim()
+            new_width = (cur_xlim[1] - cur_xlim[0]) * scale_factor
+            new_height = (cur_ylim[1] - cur_ylim[0]) * scale_factor
+
+            relx = (cur_xlim[1] - xdata) / (cur_xlim[1] - cur_xlim[0])
+            rely = (cur_ylim[1] - ydata) / (cur_ylim[1] - cur_ylim[0])
+            xzoom = yzoom = True
+            if wx.GetKeyState(wx.WXK_CONTROL_X):
+                yzoom = False
+            elif wx.GetKeyState(wx.WXK_CONTROL_Y):
+                xzoom = False
+            if (xzoom) and new_width * (1 - relx) > 0:
+                ax.set_xlim(
+                    [xdata - new_width * (1 - relx), xdata + new_width * (relx)])
+            if (yzoom) and new_height * (1 - rely) > 0:
+                ax.set_ylim(
+                    [ydata - new_height * (1 - rely), ydata + new_height * (rely)])
         self.canvas.draw()
 
     def init_toolbar_empty(self):
         # deprecated in 3.3.0
         pass
     def init_toolbar(self):
         toolitems = (
@@ -372,49 +236,99 @@
             ('Zoom', 'Zoom to rectangle', zoom_xpm, 'zoom'),
             ('Datatip', 'Show the data tip', cursor_xpm, 'datatip'),
             (None, None, None, None),
             ('Save', 'Save the figure', save_xpm, 'save_figure'),
             ('Copy', 'Copy to clipboard', copy_xpm, 'copy_figure'),
             (None, None, None, None),
             ('Edit', 'Edit curve', line_edit_xpm, 'edit_figure'),
+            (None, None, None, None),
+            (None, None, None, "stretch"),
+            ('Auto Scale', 'Auto Scale', more_svg, 'OnMore'),
             #(None, None, None, None),
             #('Print', 'Print the figure', print_xpm, 'print_figure'),
         )
 
         self._parent = self.canvas.GetParent()
         self.ClearTools()
         self.wx_ids = {}
         self.SetToolBitmapSize((16, 16))
         for (text, tooltip_text, image_file, callback) in toolitems:
             if text is None:
-                self.AddSeparator()
+                if callback == "stretch":
+                    self.AddStretchSpacer()
+                else:
+                    self.AddSeparator()
                 continue
             self.wx_ids[text] = wx.NewId()
+            if isinstance(image_file, list):
+                image = wx.Bitmap(to_byte(image_file))
+            else:
+                image = svg_to_bitmap(image_file, win=self)
             if text in ['Pan', 'Zoom', 'Datatip', 'Edit']:
                 self.AddCheckTool(self.wx_ids[text],
                                   text,
-                                  wx.Bitmap(to_byte(image_file)),
-                                  shortHelp=text,
-                                  longHelp=tooltip_text)
+                                  image,
+                                  disabled_bitmap=wx.NullBitmap,
+                                  short_help_string=text,
+                                  long_help_string=tooltip_text)
             else:
                 self.AddTool(self.wx_ids[text], text,
-                             wx.Bitmap(to_byte(image_file)),
-                             kind=wx.ITEM_NORMAL, shortHelp=tooltip_text)
+                             image,
+                             disabled_bitmap=wx.NullBitmap,
+                             kind=wx.ITEM_NORMAL, short_help_string=tooltip_text)
             self.Bind(wx.EVT_TOOL,
                       getattr(self, callback),
                       id=self.wx_ids[text])
 
+        self.Bind(wx.EVT_MENU, self.OnProcessMenu, id=self.ID_AUTO_SCALE_X)
+        self.Bind(wx.EVT_MENU, self.OnProcessMenu, id=self.ID_AUTO_SCALE_Y)
+        self.Bind(wx.EVT_MENU, self.OnProcessMenu, id=self.ID_AUTO_SCALE_XY)
+
         self.Realize()
 
+    def OnMore(self, event):
+        menu = wx.Menu()
+        menu.Append(self.ID_AUTO_SCALE_XY, "Auto scale")
+        menu.AppendSeparator()
+        menu.Append(self.ID_AUTO_SCALE_X, "Auto scale x-axis")
+        menu.Append(self.ID_AUTO_SCALE_Y, "Auto scale y-axis")
+
+        # line up our menu with the button
+        tb = event.GetEventObject()
+        tb.SetToolSticky(event.GetId(), True)
+        rect = tb.GetToolRect(event.GetId())
+        pt = tb.ClientToScreen(rect.GetBottomLeft())
+        pt = self.ScreenToClient(pt)
+
+        self.PopupMenu(menu, pt)
+
+        # make sure the button is "un-stuck"
+        tb.SetToolSticky(event.GetId(), False)
+
+    def OnProcessMenu(self, event):
+        eid = event.GetId()
+        if eid == self.ID_AUTO_SCALE_XY:
+            self.do_auto_scale()
+        if eid == self.ID_AUTO_SCALE_X:
+            self.do_auto_scale('x')
+        elif eid == self.ID_AUTO_SCALE_Y:
+            self.do_auto_scale('y')
+
     def OnNewFigure(self, evt):
         dp.send('shell.run',
                 command='figure();',
-                prompt=True,
+                prompt=False,
                 verbose=False,
-                debug=False)
+                debug=False,
+                history=False)
+
+    def do_auto_scale(self,axis='both'):
+        for ax in self.figure.get_axes():
+            ax.autoscale(axis=axis)
+        self.figure.canvas.draw_idle()
 
     def copy_figure(self, evt):
         # self.canvas.Copy_to_Clipboard(event=evt)
         bmp_obj = wx.BitmapDataObject()
         bmp_obj.SetBitmap(self.canvas.bitmap)
 
         if not wx.TheClipboard.IsOpened():
@@ -450,34 +364,36 @@
         action = self.actions.get(self.mode, None)
         if action is not None and hasattr(action, 'activated'):
             action.activated()
 
     def zoom(self, *args):
         """activate the zoom mode"""
         self.set_mode('zoom')
-        super(Toolbar, self).zoom(*args)
+        super().zoom(*args)
 
     def pan(self, *args):
         """activated the pan mode"""
         self.set_mode('pan')
-        super(Toolbar, self).pan(*args)
+        super().pan(*args)
 
     def OnBack(self, *args):
         super().back(*args)
 
     def back(self, *args):
-        if self.mode == 'datatip':
+        action = self.actions.get(self.mode, None)
+        if action is not None:
             return
         super().back(*args)
 
     def OnForward(self, *args):
         super().forward(*args)
 
     def forward(self, *args):
-        if self.mode == 'datatip':
+        action = self.actions.get(self.mode, None)
+        if action is not None:
             return
         super().forward(*args)
 
     def datatip(self, evt):
         """activate the datatip mode"""
         # disable the pan/zoom mode
         self._active = None
@@ -486,16 +402,15 @@
 
         if hasattr(self, '_idRelease'):
             self._idRelease = self.canvas.mpl_disconnect(self._idRelease)
         self.canvas.widgetlock.release(self)
         for a in self.canvas.figure.get_axes():
             a.set_navigate_mode(self._active)
 
-        for l in self.figure.gca().lines:
-            l.set_picker(5)
+        self._set_picker_all()
         if self.mode == 'datatip':
             self.set_mode('')
         else:
             self.set_mode("datatip")
         self.set_message(self.mode)
         self.datacursor.set_enable(evt.GetInt())
 
@@ -510,16 +425,15 @@
 
         if hasattr(self, '_idRelease'):
             self._idRelease = self.canvas.mpl_disconnect(self._idRelease)
         self.canvas.widgetlock.release(self)
         for a in self.canvas.figure.get_axes():
             a.set_navigate_mode(self._active)
 
-        for l in self.figure.gca().lines:
-            l.set_picker(5)
+        self._set_picker_all()
         if self.mode == "edit":
             self.set_mode("")
         else:
             self.set_mode("edit")
         self.set_message(self.mode)
 
     def set_message(self, s):
@@ -528,14 +442,17 @@
 
 
 class MatplotPanel(wx.Panel):
     clsFrame = None
     clsID_new_figure = wx.NOT_FOUND
     isInitialized = False
     kwargs = {}
+    ID_PANE_CLOSE = wx.NewId()
+    ID_PANE_CLOSE_OTHERS = wx.NewId()
+    ID_PANE_CLOSE_ALL = wx.NewId()
 
     def __init__(self, parent, title=None, num=-1, thisFig=None):
         # set the size to positive value, otherwise the toolbar will assert
         # wxpython/ext/wxWidgets/src/gtk/bitmap.cpp(539): assert ""width > 0 &&
         # height > 0"" failed in Create(): invalid bitmap size
         wx.Panel.__init__(self, parent, size=(100, 100))
         # initialize matplotlib stuff
@@ -578,81 +495,56 @@
         self.Bind(wx.EVT_CHAR_HOOK, self.OnKeyDown)
 
     def GetToolBar(self):
         """Override wxFrame::GetToolBar as we don't have managed toolbar"""
         return self.toolbar
 
     def simLoad(self, num):
-        for l in self.figure.gca().lines:
-            if hasattr(l, 'trace'):
-                sz = len(l.get_ydata())
-                for s in l.trace:
-                    if (not s) or (not s.startswith(str(num) + '.')):
-                        continue
-                    #dispatcher.send(signal='sim.trace_buf', objects=s, size=sz)
+        for ax in self.figure.get_axes():
+            for l in ax.lines:
+                if hasattr(l, 'trace'):
+                    sz = len(l.get_ydata())
+                    for s in l.trace:
+                        if (not s) or (not s.startswith(str(num) + '.')):
+                            continue
+                        #dispatcher.send(signal='sim.trace_buf', objects=s, size=sz)
 
     def _onClick(self, event):
         if event.dblclick:
             self.toolbar.home()
 
     def OnKeyDown(self, evt):
-        if self.toolbar.mode != 'datatip':
-            return
-        keycode = evt.GetKeyCode()
-        step = 1
-        if evt.ShiftDown():
-            step = 10
-        if keycode == wx.WXK_LEFT:
-            self.toolbar.datacursor.keyboard_move(True, step=step)
-        elif keycode == wx.WXK_RIGHT:
-            self.toolbar.datacursor.keyboard_move(False, step=step)
-        else:
-            evt.Skip()
+        self.toolbar.key_down(evt)
 
     def OnProcessCommand(self, evt):
         if self.toolbar.datacursor.ProcessCommand(evt.GetId()):
             self.canvas.draw()
 
-    def _create_context_menu(self, menus):
-        menu = wx.Menu()
-        for m in menus:
-            if len(m) == 0:
-                item = menu.AppendSeparator()
-            elif isinstance(m[0], str):
-                child = self._create_context_menu(m[1])
-                menu.AppendSubMenu(child, m[0])
-            elif len(m) == 3:
-                # normal item
-                item = menu.Append(m[0], m[1])
-                item.Enable(m[2])
-            elif len(m) == 4:
-                # checkable item
-                item = menu.AppendCheckItem(m[0], m[1])
-                item.Check(m[3])
-                item.Enable(m[2])
-        return menu
-
     def _show_context_menu(self):
         menus = self.toolbar.GetMenu()
         if len(menus) == 0:
             return
-        menu = self._create_context_menu(menus)
-
+        menu = build_menu_from_list(menus)
+        if self.canvas.HasCapture():
+            self.canvas.ReleaseMouse()
         mid = PopupMenu(self, menu)
         if mid > 0:
             self.toolbar.ProcessCommand(mid)
         menu.Destroy()
 
     def OnContextMenu(self, event):
         # Show menu after the current and pending event handlers have been
         # completed, otherwise it causes the following error in some system
         # (e.g., xubuntu, matplotlib 3.2.2, wx 4.1.0), and the menu doesn't show.
         # GLib-GObject-CRITICAL **: g_object_set_data: assertion 'G_IS_OBJECT
         # (object)' failed
-        wx.CallAfter(self._show_context_menu)
+        # remove the wx.CallAfter, as the problem doesn't show on xubuntu
+        # 22.04/matplotlib 3.7.1/wx 4.2.0, and on xubuntu 22.04, wx.CallAfter
+        # will cause the menu to disappear as soon as the right button is up
+        self._show_context_menu()
 
     def _onClose(self, evt):
         self.canvas.close_event()
         self.canvas.stop_event_loop()
         Gcf.destroy(self.num)
 
     def destroy(self, *args):
@@ -661,15 +553,15 @@
             wx.WakeUpIdle()
 
     def Destroy(self, *args, **kwargs):
         self.isdestory = True
         self.canvas.close_event()
         self.canvas.stop_event_loop()
         Gcf.destroy(self.num)
-        return super(MatplotPanel, self).Destroy(*args, **kwargs)
+        return super().Destroy(*args, **kwargs)
 
     def GetTitle(self):
         """return the figure title"""
         return self.title
 
     def SetTitle(self, title):
         """set the figure title"""
@@ -682,37 +574,38 @@
         """show figure"""
         if self.IsShown() is False:
             self.canvas.draw()
             dp.send('frame.show_panel', panel=self)
 
     def update_buffer(self, bufs):
         """update the data used in plot_trace"""
-        for l in self.figure.gca().lines:
-            if hasattr(l, 'trace'):
-                x = l.trace[0]
-                y = l.trace[1]
-                if x is None:
-                    if y in bufs:
-                        l.set_data(numpy.arange(len(bufs[y])), bufs[y])
-                elif x in bufs or y in bufs:
-                    xd = l.get_xdata()
-                    yd = l.get_ydata()
-                    if y in bufs:
-                        yd = bufs[y]
-                    if x in bufs:
-                        xd = bufs[x]
-                    if len(xd) != len(yd):
-                        sz = min(len(xd), len(yd))
-                        xd = xd[0:sz]
-                        yd = yd[0:sz]
-                    l.set_data(xd, yd)
-                if hasattr(l, 'autorelim') and l.autorelim:
-                    #Need both of these in order to rescale
-                    self.figure.gca().relim()
-                    self.figure.gca().autoscale_view()
+        for ax in self.figure.get_axes():
+            for l in ax.lines:
+                if hasattr(l, 'trace'):
+                    x = l.trace[0]
+                    y = l.trace[1]
+                    if x is None:
+                        if y in bufs:
+                            l.set_data(np.arange(len(bufs[y])), bufs[y])
+                    elif x in bufs or y in bufs:
+                        xd = l.get_xdata()
+                        yd = l.get_ydata()
+                        if y in bufs:
+                            yd = bufs[y]
+                        if x in bufs:
+                            xd = bufs[x]
+                        if len(xd) != len(yd):
+                            sz = min(len(xd), len(yd))
+                            xd = xd[0:sz]
+                            yd = yd[0:sz]
+                        l.set_data(xd, yd)
+                    if hasattr(l, 'autorelim') and l.autorelim:
+                        #Need both of these in order to rescale
+                        ax.relim()
+                        ax.autoscale_view()
         self.canvas.draw()
 
     def plot_trace(self, x, y, autorelim, *args, **kwargs):
         """plot and trace"""
         if y is None:
             return
         if x is None:
@@ -729,14 +622,15 @@
                 else:
                     xd = 0
                     yd = 0
             l, = self.figure.gca().plot(xd, yd, *args, **kwargs)
             l.trace = [list(x.keys())[0], list(y.keys())[0]]
         l.autorelim = autorelim
         self.canvas.draw()
+
     def set_window_title(self, label):
         pass
 
     @classmethod
     def setactive(cls, pane):
         """set the active figure"""
         if pane and isinstance(pane, MatplotPanel):
@@ -753,15 +647,21 @@
         # wxpython/ext/wxWidgets/src/gtk/bitmap.cpp(539): assert ""width > 0 &&
         # height > 0"" failed in Create(): invalid bitmap size
         dp.send('frame.add_panel',
                 panel=fig,
                 direction=direction,
                 title=fig.GetTitle(),
                 target=Gcf.get_active(),
-                minsize=(75, 75))
+                minsize=(75, 75),
+                pane_menu={'rxsignal': 'bsm.graph.pane_menu',
+                           'menu': [
+                               {'id':cls.ID_PANE_CLOSE, 'label':'Close\tCtrl+W'},
+                               {'id':cls.ID_PANE_CLOSE_OTHERS, 'label':'Close Others'},
+                               {'id':cls.ID_PANE_CLOSE_ALL, 'label':'Close All'},
+                               ]})
         return fig
 
     @classmethod
     def Initialize(cls, frame, **kwargs):
         if cls.isInitialized:
             return
         cls.isInitialized = True
@@ -771,18 +671,36 @@
                        path='File:New:Figure\tCtrl+P',
                        rxsignal='bsm.figure')
         if resp:
             cls.clsID_new_figure = resp[0][1]
 
         if cls.clsID_new_figure is not wx.NOT_FOUND:
             dp.connect(cls.ProcessCommand, 'bsm.figure')
-        dp.connect(cls.Uninitialize, 'frame.exit')
+        dp.connect(cls.Uninitialize, 'frame.exiting')
         dp.connect(cls.Initialized, 'frame.initialized')
         dp.connect(cls.setactive, 'frame.activate_panel')
         dp.connect(cls.OnBufferChanged, 'sim.buffer_changed')
+        dp.connect(cls.PaneMenu, 'bsm.graph.pane_menu')
+
+    @classmethod
+    def PaneMenu(cls, pane, command):
+        if not pane or not isinstance(pane, MatplotPanel):
+            return
+        if command == cls.ID_PANE_CLOSE:
+            dp.send(signal='frame.delete_panel', panel=pane)
+        elif command == cls.ID_PANE_CLOSE_OTHERS:
+            mgrs =  Gcf.get_all_fig_managers()
+            for mgr in mgrs:
+                if mgr == pane:
+                    continue
+                dp.send(signal='frame.delete_panel', panel=mgr)
+        elif command == cls.ID_PANE_CLOSE_ALL:
+            mgrs =  Gcf.get_all_fig_managers()
+            for mgr in mgrs:
+                dp.send(signal='frame.delete_panel', panel=mgr)
 
     @classmethod
     def Initialized(cls):
         dp.send('shell.run',
                 command='from matplotlib.pyplot import *',
                 prompt=False,
                 verbose=False,
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/lineeditor.py` & `bsmedit-3.2.9/bsmedit/bsm/lineeditor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,204 +1,192 @@
 import wx
 import wx.py.dispatcher as dp
 import numpy as np
+from .graph_common import GraphObject
 
-class LineEditor():
+class LineEditor(GraphObject):
     ID_XY_MODE = wx.NewId()
     ID_X_MODE = wx.NewId()
     ID_Y_MODE = wx.NewId()
     ID_ROUND_Y = wx.NewId()
     ID_EXPORT_TO_TERM = wx.NewId()
     ID_LINES = []
-    def __init__(self, figure, lines=None):
-        self.figure = figure
-        if lines is None:
-            self.lines = self.figure.gca().lines
-        else:
-            self.lines = lines
-        self.lines = self.lines[:]
+    def __init__(self, figure):
+        super().__init__(figure)
+
+        self.lines = {}
+        self.axes = None
 
         # marker
         # set larger zorder, so always on top
-        self.marker = self.figure.gca().plot([0], [0], marker="o", color="red", zorder=10)[0]
-
-        # cross hair
-        self.horizontal_line = self.figure.gca().axhline(color='g', lw=0.8, ls='--', zorder=10)
-        self.vertical_line = self.figure.gca().axvline(color='g', lw=0.8, ls='--', zorder=10)
-        self.show_cross_hair = False
+        self.marker = {}
 
         self.draggable = False
-        self.marker.set_visible(self.draggable)
-        self.horizontal_line.set_visible(False)
-        self.vertical_line.set_visible(False)
+        #self.marker.set_visible(self.draggable)
 
-        self.active_line_index = None
+        self.active_line = None
         self.index = None
 
         self.mode = 'x'
-        self.prev_pos = None
         self.round_y_to = 0
 
-    def set_cross_hair_visible(self, visible):
-        need_redraw = self.horizontal_line.get_visible() != visible
-        self.horizontal_line.set_visible(visible)
-        self.vertical_line.set_visible(visible)
-        #self.text.set_visible(visible)
-        return need_redraw
+    def update_marker(self):
+        # update marker
+        for g in self.marker:
+            self.marker[g].set_visible(False)
+
+        if self.draggable and self.active_line:
+            self.marker[self.active_line.axes].set_visible(True)
 
     def mouse_pressed(self, event):
         if not event.inaxes:
             return
+        axes = [a for a in self.figure.get_axes()
+                if a.in_axes(event)]
+        for g in axes:
+            if self.marker.get(g, None) is None:
+                self.marker[g] = g.plot([], [], marker="o", color="red", zorder=10)[0]
+                self.marker[g].set_visible(False)
+        self.axes = axes
+
         if event.button == 1:
             # left click
             self.draggable = True
             self.update(event)
+            self.update_marker()
         elif event.button == 3:
             self.draggable = False
-        self.marker.set_visible(self.draggable)
-        self.prev_pos = [event.xdata, event.ydata]
 
         self.figure.canvas.draw_idle()
 
     def mouse_move(self, event):
         if not event.inaxes:
-            need_redraw = self.set_cross_hair_visible(False)
-            if need_redraw:
-                self.figure.canvas.draw_idle()
             return
 
         mx, my = event.xdata, event.ydata
-        self.set_cross_hair_visible(self.show_cross_hair)
-        self.horizontal_line.set_ydata(my)
-        self.vertical_line.set_xdata(mx)
 
         if self.draggable:
+            inv = self.active_line.axes.transData.inverted()
+            mx, my = inv.transform((event.x, event.y))
             if self.round_y_to is not None:
                 my = round(my, self.round_y_to)
 
-            line = self.lines[self.active_line_index]
-            x, y = line.get_data()
+            x, y = self.active_line.get_data()
             x = x.copy()
             y = y.copy()
             mode = self.mode
             shift = wx.GetKeyState(wx.WXK_SHIFT)
             if mode == 'x' and shift:
                 mode = 'y'
             elif mode == 'y' and shift:
                 mode = 'x'
             if mode == 'x':
-                idx, _, _ = self.get_closest(line, mx, None)
+                # search the index based on x-axis only
+                idx, _, _ = self.get_closest(self.active_line, mx, None, 5)
+                if isinstance(idx, np.ndarray):
+                    idx_closest = np.argmin(np.abs(idx - self.index))
+                    idx = idx[idx_closest]
+                # search based on x and y
+                idx2, _, _ = self.get_closest(self.active_line, mx, my)
+                # find the index that is close to the current position
+                if abs(idx2 - self.index) < abs(idx - self.index):
+                    idx = idx2
+
                 if self.index > 0 and idx < self.index:
                     # move to left
                     y[idx:self.index] = y[self.index]
                     self.index = idx
                 elif self.index > 0 and idx > self.index:
                     # move to right
-                    y[self.index:idx] = y[self.index - 1]
+                    y[self.index:idx+1] = y[self.index - 1]
+                    self.index = idx
+                else:
                     self.index = idx
             elif mode == 'y':
                 y[self.index] = my
             else:
                 x[self.index] = mx
                 y[self.index] = my
-            self.marker.set_data([x[self.index]], [y[self.index]])
-            line.set_data(x, y)
+            self.marker[self.active_line.axes].set_data([x[self.index]], [y[self.index]])
+            self.active_line.set_data(x, y)
         self.figure.canvas.draw_idle()
 
     def mouse_released(self, event):
         self.draggable = False
 
-    def get_xy_dis_gain(self):
-        # the gain applied to x/y when calculate the distance between to point
-        # e.g., a data point to the mouse position
-        # for example, if the figure is square (width == height), but
-        # x range is [0, 100], and y range is [0, 0.1], the physical distance
-        # in y axis will be `ignored` as x is 1000 times larger than y.
-        xlim = self.figure.gca().get_xlim()
-        ylim = self.figure.gca().get_ylim()
-        box = self.figure.gca().get_window_extent()
-        if xlim[1] - xlim[0] == 0 or ylim[1] - ylim[0] == 0:
-            return 1, 1
-        gx = box.width / (xlim[1] - xlim[0])
-        gy = box.height / (ylim[1] - ylim[0])
-        return gx, gy
+    def update_line(self):
+        # ignore the internal lines (e.g., marker)
+        self.lines = {}
+        for g in self.axes:
+            self.lines[g] = [l for l in g.lines if l != self.marker.get(g, None)]
+
+        if self.active_line:
+            if self.active_line not in self.lines.get(self.active_line.axes, []):
+                self.active_line = None
 
     def update(self, event):
-        # ignore the first 3 lines (marker + 2 cross hair)
-        self.lines = self.figure.gca().lines[3:]
-        if self.active_line_index is None:
-            min_dis = float("inf")
-            index = -1
-            gx, gy = self.get_xy_dis_gain()
-            for i, line in enumerate(self.lines):
-                if not line.get_visible():
-                    continue
-                _, x, y = self.get_closest(line, event.xdata, event.ydata)
-                dis = (x-event.xdata)**2 * gx**2 + (y-event.ydata)**2 * gy**2
-                if dis < min_dis:
-                    min_dis = dis
-                    index = i
-            if index >= 0:
-                self.active_line_index = index
-        if self.active_line_index is None:
+        self.update_line()
+        if self.active_line is None:
+            active_line, _ = self.get_closest_line(self.axes, event.x, event.y)
+            if active_line:
+                self.active_line = active_line
+        if self.active_line is None:
             return
-        line = self.lines[self.active_line_index]
-        self.index, x, y = self.get_closest(line, event.xdata, event.ydata)
-        self.marker.set_data([x], [y])
-
-    def get_closest(self, line, mx, my):
-        """return the index of closed data point"""
-        x, y = line.get_data()
-        if mx is None and my is None:
-            return -1
-        if my is None:
-            mini = np.argmin((x-mx)**2)
-        elif mx is None:
-            mini = np.argmin((y-my)**2)
-        else:
-            gx, gy = self.get_xy_dis_gain()
-            mini = np.argmin((x-mx)**2 * gx**2 + (y-my)**2 * gy**2)
-        return mini, x[mini], y[mini]
+        inv = self.active_line.axes.transData.inverted()
+        mx, my = inv.transform((event.x, event.y))
+        self.index, x, y = self.get_closest(self.active_line, mx, my)
+        self.marker[self.active_line.axes].set_data([x], [y])
 
     def key_pressed(self, event):
         """Callback for key presses."""
         if not event.inaxes:
             return
         if event.key == 'escape':
-            self.active_line_index = None
-            self.marker.set_visible(False)
+            if self.active_line:
+                self.marker[self.active_line.axes].set_visible(False)
+            self.active_line = None
+            self.draggable = False
             self.figure.canvas.draw_idle()
 
     def activated(self):
         pass
 
     def deactivated(self):
         self.draggable = False
-        self.marker.set_visible(self.draggable)
-        self.horizontal_line.set_visible(False)
-        self.vertical_line.set_visible(False)
+        if self.active_line:
+            if self.active_line.axes in self.marker:
+                self.marker[self.active_line.axes].set_visible(False)
 
     def GetMenu(self):
-        cmd = [[self.ID_XY_MODE, 'x/y mode', True, self.mode == ''],
-               [self.ID_X_MODE, 'x only mode', True, self.mode == 'x'],
-               [self.ID_Y_MODE, 'y only mode', True, self.mode == 'y'],
-               [self.ID_ROUND_Y, 'Round y to', True, self.round_y_to != None],
-               [],
+        cmd = [{'type': wx.ITEM_CHECK, 'id': self.ID_XY_MODE, 'label': 'x/y mode',
+                'check': self.mode == ''},
+               {'type': wx.ITEM_CHECK, 'id': self.ID_X_MODE, 'label': 'x only mode',
+                'check': self.mode == 'x'},
+               {'type': wx.ITEM_CHECK, 'id': self.ID_Y_MODE, 'label': 'y only mode',
+                'check': self.mode == 'y'},
+               {'type': wx.ITEM_CHECK, 'id': self.ID_ROUND_Y, 'label': 'Round y to',
+                'check': self.round_y_to is not None},
+               {'type': wx.ITEM_SEPARATOR},
               ]
 
-        self.lines = self.figure.gca().lines[3:]
-        lines = []
-        lines.append([self.ID_EXPORT_TO_TERM, 'Export active line to shell ...', self.active_line_index != None])
-        lines.append([])
-        for i, line in enumerate(self.lines):
-            while i >= len(self.ID_LINES):
-                self.ID_LINES.append(wx.NewId())
-            lines.append([self.ID_LINES[i], line.get_label(), True, self.active_line_index == i])
-        if lines:
-            cmd.append(['Lines', lines])
+        self.update_line()
+        menu_lines = []
+        menu_lines.append({'id': self.ID_EXPORT_TO_TERM, 'label': 'Export active line to shell ...',
+                      'enable': self.active_line is not None})
+        menu_lines.append({'type': wx.ITEM_SEPARATOR})
+        i = 0
+        for _, lines in self.lines.items():
+            for line in lines:
+                while i >= len(self.ID_LINES):
+                    self.ID_LINES.append(wx.NewId())
+                menu_lines.append({'type': wx.ITEM_CHECK, 'id': self.ID_LINES[i],
+                              'label': line.get_label(), 'check': self.active_line == line})
+                i += 1
+        if menu_lines:
+            cmd.append({'type': wx.ITEM_DROPDOWN, 'label': 'Lines', 'items': menu_lines})
         return cmd
 
     def ProcessCommand(self, cmd):
         if cmd == self.ID_XY_MODE:
             self.mode = ''
         elif cmd == self.ID_X_MODE:
             self.mode = 'x'
@@ -217,21 +205,31 @@
             try:
                 ry = int(ry)
             except:
                 ry = None
             self.round_y_to = ry
 
         elif cmd == self.ID_EXPORT_TO_TERM:
-            x, y = self.lines[self.active_line_index].get_data()
+            x, y = self.active_line.get_data()
             np.save('_lineeditor.npy', (x, y))
             dp.send('shell.run',
                     command='le_data = np.load("_lineeditor.npy", allow_pickle=True)',
                     prompt=False,
                     verbose=False,
                     history=False)
             dp.send('shell.run',
                     command='le_data',
                     prompt=True,
                     verbose=True,
                     history=False)
         elif cmd in self.ID_LINES:
-            self.active_line_index = self.ID_LINES.index(cmd)
+            i = 0
+            for _, lines in self.lines.items():
+                for line in lines:
+                    if i == self.ID_LINES.index(cmd):
+                        self.active_line = line
+                        break
+                    i += 1
+                else:
+                    # if not found in lines, keep searching
+                    continue
+                break
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/misctools.py` & `bsmedit-3.2.9/bsmedit/mainframe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,485 +1,519 @@
-import pydoc
-import os
-import time
-import traceback
+"""Subclass of mainFrame, which is generated by wxFormBuilder."""
+
 import sys
+import importlib
+import traceback
+import json
+import datetime
 import six
+import six.moves
 import wx
-import wx.lib.agw.aui as aui
+import wx.py
 import wx.py.dispatcher as dp
-import wx.html2 as html
-import wx.svg
-from .dirtreectrl import DirTreeCtrl, Directory
-from .bsmxpm import backward_svg, forward_svg, goup_xpm, home_xpm
-from .autocomplete import AutocompleteTextCtrl
-from .utility import FastLoadTreeCtrl, svg_to_bitmap
-
-from .. import to_byte
-
-html_template = '''
-<html>
-    <head>
-        <title>%(title)s</title>
-    </head>
-    <body>
-    <FONT FACE= "Courier New">
-    <pre>
-%(message)s
-    </pre>
-    </body>
-</html>
-'''
+import wx.adv
+from .aui import aui
+from .frameplus import FramePlus
+from .mainframexpm import  bsmedit_svg
+from . import __version__
+from .bsm.utility import PopupMenu, svg_to_bitmap, build_menu_from_list
+from .bsm import auto_load_module
+
+class FileDropTarget(wx.FileDropTarget):
+    def __init__(self):
+        wx.FileDropTarget.__init__(self)
+
+    def OnDropFiles(self, x, y, filenames):
+        for fname in filenames:
+            wx.CallAfter(dp.send, signal='frame.file_drop', filename=fname)
+        return True
+
+class TaskBarIcon(wx.adv.TaskBarIcon):
+    TBMENU_RESTORE = wx.NewId()
+    TBMENU_CLOSE = wx.NewId()
+    TBMENU_CHANGE = wx.NewId()
+    TBMENU_REMOVE = wx.NewId()
+
+    def __init__(self, frame, icon):
+        wx.adv.TaskBarIcon.__init__(self, iconType=wx.adv.TBI_DOCK)
+        self.frame = frame
+
+        # Set the image
+        self.SetIcon(icon, "bsmedit")
+        self.imgidx = 1
+
+        # bind some events
+        #self.Bind(wx.EVT_TASKBAR_LEFT_DCLICK, self.OnTaskBarActivate)
+        self.Bind(wx.EVT_MENU, self.OnTaskBarActivate, id=self.TBMENU_RESTORE)
+        self.Bind(wx.EVT_MENU, self.OnTaskBarClose, id=self.TBMENU_CLOSE)
+
+
+    def CreatePopupMenu(self):
+        """
+        This method is called by the base class when it needs to popup
+        the menu for the default EVT_RIGHT_DOWN event.  Just create
+        the menu how you want it and return it from this function,
+        the base class takes care of the rest.
+        """
+        menu = wx.Menu()
+        menu.Append(self.TBMENU_RESTORE, "Restore bsmedit")
+        menu.Append(self.TBMENU_CLOSE, "Close bsmedit")
+        return menu
+
+
+    def MakeIcon(self, img):
+        """
+        The various platforms have different requirements for the
+        icon size...
+        """
+        if "wxMSW" in wx.PlatformInfo:
+            img = img.Scale(16, 16)
+        elif "wxGTK" in wx.PlatformInfo:
+            img = img.Scale(22, 22)
+        # wxMac can be any size upto 128x128, so leave the source img alone....
+        icon = wx.Icon(img.ConvertToBitmap())
+        return icon
+
+
+    def OnTaskBarActivate(self, evt):
+        if self.frame.IsIconized():
+            self.frame.Iconize(False)
+        if not self.frame.IsShown():
+            self.frame.Show(True)
+        self.frame.Raise()
+
+
+    def OnTaskBarClose(self, evt):
+        wx.CallAfter(self.frame.Close)
+
+class MultiDimensionalArrayEncoder(json.JSONEncoder):
+    def encode(self, obj):
+        def hint_tuples(item):
+            if isinstance(item, tuple):
+                return {'__tuple__': True, 'items': item}
+            if isinstance(item, list):
+                return [hint_tuples(e) for e in item]
+            if isinstance(item, dict):
+                return {key: hint_tuples(value) for key, value in item.items()}
+            else:
+                return item
+
+        return super().encode(hint_tuples(obj))
+
+def hinted_tuple_hook(obj):
+    if '__tuple__' in obj:
+        return tuple(obj['items'])
+    else:
+        return obj
+
+class MainFrame(FramePlus):
+
+    ID_VM_RENAME = wx.NewId()
+    ID_CONTACT = wx.NewId()
+
+    def __init__(self, parent, **kwargs):
+        FramePlus.__init__(self,
+                           parent,
+                           title='bsmedit',
+                           size=wx.Size(800, 600),
+                           style=wx.DEFAULT_FRAME_STYLE | wx.TAB_TRAVERSAL)
+        self.InitMenu()
+        self._mgr.SetAGWFlags(self._mgr.GetAGWFlags()
+                              | aui.AUI_MGR_ALLOW_ACTIVE_PANE
+                              | aui.AUI_MGR_SMOOTH_DOCKING
+                              | aui.AUI_MGR_USE_NATIVE_MINIFRAMES
+                              | aui.AUI_MGR_LIVE_RESIZE)
+        # set mainframe icon
+        icon = wx.Icon()
+        icon.CopyFromBitmap(svg_to_bitmap(bsmedit_svg, win=self))
+        self.SetIcon(icon)
+
+        if 'wxMac' in wx.PlatformInfo:
+            icon.CopyFromBitmap(svg_to_bitmap(bsmedit_svg, 1024, 1024, win=self))
+            self.tbicon = TaskBarIcon(self, icon)
+
+        # status bar
+        self.statusbar = wx.StatusBar(self)
+        self.SetStatusBar(self.statusbar)
+        self.statusbar_width = [-1]
+        self.statusbar.SetStatusWidths(self.statusbar_width)
+
+        # persistent configuration
+        conf = kwargs.get('config', 'bsmedit')
+        self.config = wx.FileConfig(conf, style=wx.CONFIG_USE_LOCAL_FILE)
+
+        # recent file list
+        self.filehistory = wx.FileHistory(8)
+        self.config.SetPath('/FileHistory')
+        self.filehistory.Load(self.config)
+        self.filehistory.UseMenu(self.menuRecentFiles)
+        self.filehistory.AddFilesToMenu()
+        self.Bind(wx.EVT_MENU_RANGE,
+                  self.OnMenuFileHistory,
+                  id=wx.ID_FILE1,
+                  id2=wx.ID_FILE9)
+
+        self.closing = False
+
+        # Create & Link the Drop Target Object to main window
+        self.SetDropTarget(FileDropTarget())
+
+        self.Bind(wx.EVT_ACTIVATE, self.OnActivate)
+        self.Bind(aui.EVT_AUI_PANE_ACTIVATED, self.OnPaneActivated)
+        dp.connect(self.SetPanelTitle, 'frame.set_panel_title')
+        dp.connect(self.ShowStatusText, 'frame.show_status_text')
+        dp.connect(self.AddFileHistory, 'frame.add_file_history')
+        dp.connect(self.SetConfig, 'frame.set_config')
+        dp.connect(self.GetConfig, 'frame.get_config')
+
+        # append sys path
+        sys.path.append('.')
+        for p in kwargs.get('path', []):
+            sys.path.append(p)
+
+        self.bsm_packages = auto_load_module
+        self.addon = {}
+        self.InitAddOn(kwargs.get('module', ()), debug=kwargs.get('debug', False))
+
+        # initialization done, broadcasting the message so plugins can do some
+        # after initialization processing.
+        dp.send('frame.initialized')
+        # load the perspective
+        if not kwargs.get('ignore_perspective', False):
+            perspective = self.GetConfig('mainframe', 'perspective')
+            if perspective and not wx.GetKeyState(wx.WXK_SHIFT):
+                self._mgr.LoadPerspective(perspective)
+                self.UpdatePaneMenuLabel()
+
+        self.Bind(aui.EVT_AUINOTEBOOK_TAB_RIGHT_DOWN, self.OnPageRightDown)
+        self.Bind(wx.EVT_RIGHT_DOWN, self.OnRightDown)
+
+    def InitMenu(self):
+        """initialize the menubar"""
+        menubar = wx.MenuBar()
+        self.SetMenuBar(menubar)
+
+        self.AddMenu('&File:New', kind="Popup", autocreate=True)
+        self.AddMenu('&File:Open', kind="Popup")
+        self.AddMenu('&File:Sep', kind="Separator")
+        self.AddMenu('&File:Recent Files', kind="Popup")
+        self.menuRecentFiles = self.GetMenu(['File', 'Recent Files'])
+        self.AddMenu('&File:Sep', kind="Separator")
+        self.AddMenu('&File:&Quit', id=wx.ID_CLOSE)
+
+        self.AddMenu('&View:Toolbars', kind="Popup", autocreate=True)
+        self.AddMenu('&View:Sep', kind="Separator")
+        self.AddMenu('&View:Panels', kind="Popup")
+
+        self.AddMenu('&Tools', kind="Popup", autocreate=True)
+
+        self.AddMenu('&Help:&Home', id=wx.ID_HOME, autocreate=True)
+        self.ID_CONTACT = self.AddMenu('&Help:&Contact')
+        self.AddMenu('&Help:Sep', kind="Separator")
+        self.AddMenu('&Help:About', id=wx.ID_ABOUT)
+
+        # Connect Events
+        self.Bind(wx.EVT_MENU, self.OnFileQuit, id=wx.ID_CLOSE)
+        self.Bind(wx.EVT_MENU, self.OnHelpHome, id=wx.ID_HOME)
+        self.Bind(wx.EVT_MENU, self.OnHelpContact, id=self.ID_CONTACT)
+        self.Bind(wx.EVT_MENU, self.OnHelpAbout, id=wx.ID_ABOUT)
+
+    def InitAddOn(self, modules, debug=False):
+        if not modules:
+            # load all modules
+            modules = ["default"]
+
+        for module in modules:
+            module = module.split('+')
+            options = {'debug': debug}
+            if len(module) == 2:
+                if all([c in 'htblr' for c in module[1]]):
+                    if 'h' in module[1]:
+                        options['active'] = False
+                    if 't' in module[1]:
+                        options['direction'] = 'Top'
+                    if 'b' in module[1]:
+                        options['direction'] = 'bottom'
+                    if 'l' in module[1]:
+                        options['direction'] = 'left'
+                    if 'r' in module[1]:
+                        options['direction'] = 'right'
+                options['data'] = module[1]
+            module = module[0]
+            if module == 'default':
+                module = self.bsm_packages
+            else:
+                module = [module]
+            for pkg in module:
+                if pkg in self.bsm_packages:
+                    # module in bsm
+                    pkg = 'bsmedit.bsm.%s' % pkg
+
+                if pkg in self.addon:
+                    # already loaded
+                    continue
+                self.addon[pkg] = False
+                try:
+                    mod = importlib.import_module(pkg)
+                except ImportError:
+                    traceback.print_exc(file=sys.stdout)
+                else:
+                    if hasattr(mod, 'bsm_initialize'):
+                        mod.bsm_initialize(self, **options)
+                        self.addon[pkg] = True
+                    else:
+                        print("Error: Invalid module: %s" % pkg)
+
+    def AddFileHistory(self, filename):
+        """add the file to recent file list"""
+        self.config.SetPath('/FileHistory')
+        self.filehistory.AddFileToHistory(filename)
+        self.filehistory.Save(self.config)
+        self.config.Flush()
+
+    def SetConfig(self, group, **kwargs):
+        if not group.startswith('/'):
+            group = '/' + group
+        for key, value in six.iteritems(kwargs):
+            if key in ['signal', 'sender']:
+                # reserved key for dp.send
+                continue
+            if not isinstance(value, str):
+                # add sign to indicate that the value needs to be deserialize
+                enc = MultiDimensionalArrayEncoder()
+                value = '__bsm__' + enc.encode(value)
+            self.config.SetPath(group)
+            self.config.Write(key, value)
+
+    def GetConfig(self, group, key=None):
+        if not group.startswith('/'):
+            group = '/' + group
+        if self.config.HasGroup(group):
+            self.config.SetPath(group)
+            if key is None:
+                rst = {}
+                more, k, index = self.config.GetFirstEntry()
+                while more:
+                    value = self.config.Read(k)
+                    if value.startswith('__bsm__'):
+                        value = json.loads(value[7:], object_hook=hinted_tuple_hook)
+                    rst[k] = value
+                    more, k, index = self.config.GetNextEntry(index)
+                return rst
+
+            if self.config.HasEntry(key):
+                value = self.config.Read(key)
+                if value.startswith('__bsm__'):
+                    value = json.loads(value[7:])
+                return value
+        return None
+
+    def OnPageRightDown(self, evt):
+        # get the index inside the current tab control
+        idx = evt.GetSelection()
+        tabctrl = evt.GetEventObject()
+        tabctrl.SetSelection(idx)
+        page = tabctrl.GetPage(idx)
+        self.RenamePanel(page)
 
+    def OnRightDown(self, evt):
+        evt.Skip()
 
-class HelpPanel(wx.Panel):
-    def __init__(self, parent):
-        wx.Panel.__init__(self, parent)
+        part = self._mgr.HitTest(*evt.GetPosition())
+        if not part or part.pane.IsNotebookControl():
+            return
 
-        self.html = html.WebView.New(self)
+        self.RenamePanel(part.pane.window)
 
-        agwStyle = aui.AUI_TB_OVERFLOW | aui.AUI_TB_PLAIN_BACKGROUND
-        self.tb = aui.AuiToolBar(self, agwStyle=agwStyle)
-        self.tb.AddSimpleTool(wx.ID_BACKWARD, 'Back',
-                              svg_to_bitmap(backward_svg),
-                              'Go the previous page')
-
-        self.tb.AddSimpleTool(wx.ID_FORWARD, 'Forward',
-                              svg_to_bitmap(forward_svg),
-                              'Go to the next page')
-        self.search = AutocompleteTextCtrl(self.tb, completer=self.completer)
-        item = self.tb.AddControl(self.search)
-        item.SetProportion(1)
-        self.tb.Realize()
-
-        # Setup the layout
-        sizer = wx.BoxSizer(wx.VERTICAL)
-        sizer.Add(self.tb, 0, wx.ALL | wx.EXPAND, 0)
-        sizer.Add(self.html, 1, wx.ALL | wx.EXPAND, 0)
-        self.SetSizer(sizer)
-
-        self.history = []
-        self.history_index = -1
-        self.findStr = ""
-        self.findFlags = html.WEBVIEW_FIND_DEFAULT | html.WEBVIEW_FIND_WRAP
-
-        self.Bind(wx.EVT_TEXT_ENTER, self.OnDoSearch, self.search)
-        self.Bind(html.EVT_WEBVIEW_NAVIGATING, self.OnWebViewNavigating,
-                  self.html)
-        self.Bind(wx.EVT_UPDATE_UI, self.OnUpdateUI)
-        self.Bind(wx.EVT_TOOL, self.OnBack, id=wx.ID_BACKWARD)
-        self.Bind(wx.EVT_TOOL, self.OnForward, id=wx.ID_FORWARD)
-        self.Bind(wx.EVT_TOOL, self.OnShowFind, id=wx.ID_FIND)
-
-        accel = [(wx.ACCEL_CTRL, ord('F'), wx.ID_FIND)]
-        self.accel = wx.AcceleratorTable(accel)
-        self.SetAcceleratorTable(self.accel)
-
-    def OnShowFind(self, evt):
-        self.html.Find("")
-        findData = wx.FindReplaceData()
-        dlg = wx.FindReplaceDialog(self, findData, "Find")
-        dlg.findData = findData
-        dlg.Bind(wx.EVT_FIND, self.OnFind)
-        dlg.Bind(wx.EVT_FIND_NEXT, self.OnFind)
-        dlg.Show(True)
-
-    def OnFind(self, evt):
-        self.findStr = evt.GetFindString()
-        flags = evt.GetFlags()
-        self.findFlags = html.WEBVIEW_FIND_DEFAULT | html.WEBVIEW_FIND_WRAP
-        if wx.FR_WHOLEWORD & flags:
-            self.findFlags |= html.WEBVIEW_FIND_ENTIRE_WORD
-        if wx.FR_MATCHCASE & flags:
-            self.findFlags |= html.WEBVIEW_FIND_MATCH_CASE
-        if not (wx.FR_DOWN & flags):
-            self.findFlags |= html.WEBVIEW_FIND_BACKWARDS
-        self.html.Find(self.findStr, self.findFlags)
-
-    def completer(self, query):
-        response = dp.send(signal='shell.auto_complete_list', command=query)
-        if response:
-            root = query[0:query.rfind('.') + 1]
-            remain = query[query.rfind('.') + 1:]
-            remain = remain.lower()
-            objs = [o for o in response[0][1] if o.lower().startswith(remain)]
-            return objs, objs, len(query) - len(root)
-        return [], [], 0
-
-    def add_history(self, command):
-        if not self.history or self.history[-1] != command:
-            self.history.append(command)
-            self.history_index = -1
-
-    def show_help(self, command, addhistory=True):
-        try:
-            strhelp = pydoc.plain(pydoc.render_doc(str(command), "Help on %s"))
-            htmlpage = html_template % ({'title': '', 'message': strhelp})
-            self.html.SetPage(htmlpage, '')
-            # do not use SetValue since it will trigger the text update event, which
-            # will popup the auto complete list window
-            self.search.ChangeValue(command)
-            if addhistory:
-                self.add_history(command)
-        except:
-            traceback.print_exc(file=sys.stdout)
-
-    def OnDoSearch(self, evt):
-        command = self.search.GetValue()
-        self.show_help(command)
-
-    def OnWebViewNavigating(self, evt):
-        # this event happens prior to trying to get a resource
-        strURL = evt.GetURL()
-        if strURL[:8] == 'bsmhelp:':
-            # This is how you can cancel loading a page.
-            evt.Veto()
-            command = strURL[8:]
-            self.show_help(command)
-
-    def OnUpdateUI(self, event):
-        idx = event.GetId()
-        h_idx = -1
-        h_len = len(self.history)
-        if h_len > 0:
-            h_idx = self.history_index % h_len
-        if idx == wx.ID_FORWARD:
-            event.Enable(0 <= h_idx < h_len - 1)
-        elif idx == wx.ID_BACKWARD:
-            event.Enable(h_idx > 0)
-
-    def OnBack(self, event):
-        # the button is only enabled when history_index>0
-        self.history_index -= 1
-        command = self.history[self.history_index]
-        self.show_help(command, False)
-
-    def OnForward(self, event):
-        # the button is only enable when history_index hasn't reached the last
-        # one
-        self.history_index += 1
-        command = self.history[self.history_index]
-        self.show_help(command, False)
-
-
-class HistoryPanel(wx.Panel):
-    ID_EXECUTE = wx.NewId()
-    TIME_STAMP_HEADER = "#bsm"
+    def RenamePanel(self, panel):
+        if not panel:
+            return
+        menu = wx.Menu()
+        menu.Append(self.ID_VM_RENAME, "&Rename")
+        pane_menu = None
+        if panel in self.paneMenu:
+            menu.AppendSeparator()
+            pane_menu = self.paneMenu[panel]
+            build_menu_from_list(pane_menu['menu'], menu)
+        command = PopupMenu(self, menu)
+        if command == self.ID_VM_RENAME:
+            pane = self._mgr.GetPane(panel)
+            if not pane:
+                return
+            name = pane.caption
+            name = wx.GetTextFromUser("Type in the name:", "Input Name", name,
+                                      self)
+            # when user click 'cancel', name will be empty, ignore it.
+            if name and name != pane.caption:
+                self.SetPanelTitle(pane.window, name)
+        elif command != 0 and pane_menu is not None:
+            for m in pane_menu['menu']:
+                if command == m.get('id', None):
+                    dp.send(signal=pane_menu['rxsignal'], command=command, pane=panel)
+                    break
+
+    def UpdatePaneMenuLabel(self):
+        # update the menu
+        for (pid, panel) in six.iteritems(self.paneAddon):
+            pathlist = panel['path'].split(':')
+            menuitem = self.GetMenu(pathlist[:-1])
+            if not menuitem:
+                continue
+            pane = self._mgr.GetPane(panel['panel'])
+            item = menuitem.FindItemById(pid)
+            if item and pane.caption != item.GetItemLabelText():
+                item.SetItemLabel(pane.caption)
+
+    def OnCloseWindow(self, evt):
+        self.tbicon.Destroy()
+        evt.Skip()
+
+    def OnClose(self, event):
+        """close the main program"""
+        dp.send('frame.closing', event=event)
+        if event.GetVeto():
+            return
+        self.closing = True
+        dp.send('frame.exiting')
+        self.SetConfig('mainframe', perspective=self._mgr.SavePerspective())
+        dp.send('frame.exit')
+        self.config.Flush()
+        super().OnClose(event)
+
+    def ShowStatusText(self, text, index=0, width=-1):
+        """set the status text"""
+        if index >= len(self.statusbar_width):
+            exd = [0] * (index + 1 - len(self.statusbar_width))
+            self.statusbar_width.extend(exd)
+            self.statusbar.SetFieldsCount(index + 1)
+        if self.statusbar_width[index] < width:
+            self.statusbar_width[index] = width
+            self.statusbar.SetStatusWidths(self.statusbar_width)
+        self.statusbar.SetStatusText(text, index)
 
-    def __init__(self, parent):
-        wx.Panel.__init__(self, parent)
-        style = wx.TR_DEFAULT_STYLE | wx.TR_HIDE_ROOT |wx.TR_MULTIPLE |\
-                wx.TR_HAS_VARIABLE_ROW_HEIGHT
-        # no need to sort the commands, as they are naturally sorted by
-        # execution time
-        self.tree = FastLoadTreeCtrl(self,
-                                     getchildren=self.get_children,
-                                     style=style,
-                                     sort=False)
-        self.history = {}
-        sizer = wx.BoxSizer(wx.VERTICAL)
-        sizer.Add(self.tree, 1, wx.ALL | wx.EXPAND, 0)
-        self.SetSizer(sizer)
-        dp.connect(receiver=self.AddHistory, signal='Shell.addHistory')
-        self.root = self.tree.AddRoot('The Root Item')
-        self.Bind(wx.EVT_TREE_ITEM_ACTIVATED, self.OnActivate, self.tree)
-        self.Bind(wx.EVT_TREE_ITEM_RIGHT_CLICK, self.OnRightClick, self.tree)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent, id=wx.ID_COPY)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent, id=wx.ID_CUT)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent, id=self.ID_EXECUTE)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent, id=wx.ID_DELETE)
-        self.Bind(wx.EVT_MENU, self.OnProcessEvent, id=wx.ID_CLEAR)
-
-        accel = [
-            (wx.ACCEL_CTRL, ord('C'), wx.ID_COPY),
-            (wx.ACCEL_CTRL, ord('X'), wx.ID_CUT),
-            (wx.ACCEL_CTRL, ord('E'), self.ID_EXECUTE),
-            (wx.ACCEL_NORMAL, wx.WXK_DELETE, wx.ID_DELETE),
-        ]
-        self.accel = wx.AcceleratorTable(accel)
-        self.SetAcceleratorTable(self.accel)
-        self.LoadHistory()
-
-    def Destroy(self):
-        dp.disconnect(receiver=self.AddHistory, signal='Shell.addHistory')
-        super(HistoryPanel, self).Destroy()
-
-    def get_children(self, item):
-        """ callback function to return the children of item """
-        if item == self.tree.GetRootItem():
-            childlist = list(six.iterkeys(self.history))
-            # sort by time-stamp
-            childlist.sort()
-            is_folder = True
-            clr = wx.Colour(100, 174, 100)
-        else:
-            stamp = self.tree.GetItemText(item)
-            childlist = self.history.get(stamp, [])
-            is_folder = False
-            clr = None
-            # free the list
-            self.history.pop(stamp, None)
-        children = []
-        for obj in reversed(childlist):
-            child = {
-                'label': obj,
-                'img': -1,
-                'imgsel': -1,
-                'data': '',
-                'color': clr
-            }
-            child['is_folder'] = is_folder
-            children.append(child)
-        return children
-
-    def LoadHistory(self):
-        resp = dp.send('frame.get_config', group='shell', key='history')
-        history = []
-        if resp and resp[0][1]:
-            history = resp[0][1]
-
-        stamp = time.strftime('#%Y/%m/%d')
-        for i in six.moves.range(len(history) - 1, -1, -1):
-            value = history[i]
-            if value.startswith(self.TIME_STAMP_HEADER):
-                stamp = value[len(self.TIME_STAMP_HEADER):]
-                self.history[stamp] = self.history.get(stamp, [])
-            elif self.history.get(stamp, None) is not None:
-                self.history[stamp].append(value)
-
-        self.tree.FillChildren(self.root)
-        item, cookie = self.tree.GetFirstChild(self.root)
-        if item.IsOk():
-            self.tree.Expand(item)
-            child, _ = self.tree.GetFirstChild(item)
-            if child.IsOk():
-                self.tree.SelectItem(child)
-                self.tree.EnsureVisible(child)
-
-    def SaveHistory(self, config):
-        """save the history"""
-        config.DeleteGroup('/CommandHistory')
-        config.SetPath('/CommandHistory')
-        (item, cookie) = self.tree.GetFirstChild(self.root)
-        pos = 0
-        while item.IsOk():
-            stamp = self.tree.GetItemText(item)
-            config.Write("item%d" % pos, self.TIME_STAMP_HEADER + stamp)
-            pos += 1
-
-            childitem, childcookie = self.tree.GetFirstChild(item)
-            if childitem.IsOk() and self.tree.GetItemText(childitem) != "...":
-                while childitem.IsOk():
-                    config.Write("item%d" % pos,
-                                 self.tree.GetItemText(childitem))
-                    childitem, childcookie = self.tree.GetNextChild(
-                        item, childcookie)
-                    pos = pos + 1
-            # save the unexpanded folder
-            for child in self.history.get(stamp, []):
-                config.Write("item%d" % pos, child)
-                pos = pos + 1
-
-            (item, cookie) = self.tree.GetNextChild(self.root, cookie)
-
-    def AddHistory(self, command, stamp=""):
-        """ add history to treectrl """
-        command = command.strip()
-        if not command:
+    def OnActivate(self, event):
+        if not self.closing:
+            dp.send('frame.activate', activate=event.GetActive())
+        event.Skip()
+
+    def OnPaneActivated(self, event):
+        """notify the window managers that the panel is activated"""
+        if self.closing:
             return
-        if not stamp:
-            stamp = time.strftime('#%Y/%m/%d')
+        pane = event.GetPane()
+        if isinstance(pane, aui.auibook.AuiNotebook):
+            window = pane.GetCurrentPage()
+        else:
+            window = pane
 
-        # search the time stamp
-        pos = 0
-        item, cookie = self.tree.GetFirstChild(self.root)
-        while item.IsOk():
-            if self.tree.GetItemText(item) == stamp:
-                break
-            elif self.tree.GetItemText(item) > stamp:
-                item = self.tree.InsertItemBefore(self.root, pos, stamp)
-                self.tree.SetItemTextColour(item, wx.Colour(100, 174, 100))
-                break
-            pos = pos + 1
-            (item, cookie) = self.tree.GetNextChild(self.root, cookie)
-        # not find the time stamp, create one
-        if not item.IsOk():
-            item = self.tree.PrependItem(self.root, stamp)
-            self.tree.SetItemTextColour(item, wx.Colour(100, 174, 100))
-        # append the history
-        if item.IsOk():
-            self.tree.Expand(item)
-            child = self.tree.PrependItem(item, command)
-            self.tree.EnsureVisible(child)
+        dp.send('frame.activate_panel', pane=window)
 
-    def OnActivate(self, event):
-        item = event.GetItem()
-        if not self.tree.ItemHasChildren(item):
-            command = self.tree.GetItemText(item)
-            dp.send(signal='shell.run', command=command)
+    def SetPanelTitle(self, pane, title):
+        """set the panel title"""
+        if pane:
+            info = self._mgr.GetPane(pane)
+            if info and info.IsOk() and info.caption != title:
+                info.Caption(title)
+                self._mgr.RefreshPaneCaption(pane)
+                self.UpdatePaneMenuLabel()
+
+    # Handlers for mainFrame events.
+    def OnFileQuit(self, event):
+        """close the program"""
+        self.Close(True)
+
+    def OnHelpHome(self, event):
+        """go to homepage"""
+        wx.BeginBusyCursor()
+        import webbrowser
+        webbrowser.open("http://bsmedit.feiyilin.com")
+        wx.EndBusyCursor()
+
+    def OnHelpContact(self, event):
+        """send email"""
+        wx.BeginBusyCursor()
+        import webbrowser
+        webbrowser.open("mail:tq@feiyilin.com")
+        wx.EndBusyCursor()
+
+    def OnHelpAbout(self, event):
+        """show about dialog"""
+        dlg = AboutDialog(self)
+        dlg.ShowModal()
+        dlg.Destroy()
+
+    def OnMenuFileHistory(self, event):
+        """open the recent file"""
+        fileNum = event.GetId() - wx.ID_FILE1
+        path = self.filehistory.GetHistoryFile(fileNum)
+        self.filehistory.AddFileToHistory(path)
+        dp.send('frame.file_drop', filename=path)
 
-    def OnRightClick(self, event):
-        menu = wx.Menu()
-        menu.Append(wx.ID_COPY, "Copy\tCtrl+C")
-        menu.Append(wx.ID_CUT, "Cut\tCtrl+X")
-        menu.Append(self.ID_EXECUTE, "Evaluate\tCtrl+E")
-        menu.AppendSeparator()
-        menu.AppendSeparator()
-        menu.Append(wx.ID_DELETE, "Delete\tDel")
-        menu.Append(wx.ID_CLEAR, "Clear history")
-        self.PopupMenu(menu)
-        menu.Destroy()
-
-    def OnProcessEvent(self, event):
-        items = self.tree.GetSelections()
-        cmd = []
-        for item in items:
-            cmd.append(self.tree.GetItemText(item))
-        evtId = event.GetId()
-        if evtId in (wx.ID_COPY, wx.ID_CUT):
-            clipData = wx.TextDataObject()
-            clipData.SetText("\n".join(cmd))
-            wx.TheClipboard.Open()
-            wx.TheClipboard.SetData(clipData)
-            wx.TheClipboard.Close()
-            if evtId == wx.ID_CUT:
-                for item in items:
-                    if self.tree.ItemHasChildren(item):
-                        self.tree.DeleteChildren(item)
-                    self.tree.Delete(item)
-        elif evtId == self.ID_EXECUTE:
-            for c in cmd:
-                dp.send(signal='shell.run', command=c)
-        elif evtId == wx.ID_DELETE:
-            for item in items:
-                if self.tree.ItemHasChildren(item):
-                    self.tree.DeleteChildren(item)
-                self.tree.Delete(item)
-        elif evtId == wx.ID_CLEAR:
-            self.tree.DeleteAllItems()
 
+class AboutDialog(wx.Dialog):
+    def __init__(self, parent):
+        wx.Dialog.__init__(self,
+                           parent,
+                           title="About bsmedit",
+                           style=wx.DEFAULT_DIALOG_STYLE)
 
-class DirPanel(wx.Panel):
+        szAll = wx.BoxSizer(wx.VERTICAL)
 
-    ID_GOTO_PARENT = wx.NewId()
-    ID_GOTO_HOME = wx.NewId()
+        self.panel = wx.Panel(self, style=wx.TAB_TRAVERSAL)
+        self.panel.SetBackgroundColour(wx.WHITE)
 
-    def __init__(self, parent):
-        wx.Panel.__init__(self, parent)
+        szPanelAll = wx.BoxSizer(wx.HORIZONTAL)
 
-        agwStyle = aui.AUI_TB_OVERFLOW | aui.AUI_TB_PLAIN_BACKGROUND
-        self.tb = aui.AuiToolBar(self, agwStyle=agwStyle)
-        self.tb.AddSimpleTool(self.ID_GOTO_PARENT, 'Parent',
-                              wx.Bitmap(to_byte(goup_xpm)), 'Parent folder')
-        self.tb.AddSimpleTool(self.ID_GOTO_HOME, 'Home',
-                              wx.Bitmap(to_byte(home_xpm)), 'Current folder')
-        self.tb.Realize()
-        self.dirtree = DirTreeCtrl(self,
-                                   style=wx.TR_DEFAULT_STYLE
-                                   | wx.TR_HAS_VARIABLE_ROW_HEIGHT
-                                   | wx.TR_HIDE_ROOT)
-        self.dirtree.SetRootDir(os.getcwd())
-        self.box = wx.BoxSizer(wx.VERTICAL)
-        self.box.Add(self.tb, 0, wx.EXPAND, 0)
-        #self.box.Add(wx.StaticLine(self), 0, wx.EXPAND)
-        self.box.Add(self.dirtree, 1, wx.EXPAND)
-
-        self.box.Fit(self)
-        self.SetSizer(self.box)
-
-        self.Bind(wx.EVT_TOOL, self.OnGotoHome, id=self.ID_GOTO_HOME)
-        self.Bind(wx.EVT_TOOL, self.OnGotoParent, id=self.ID_GOTO_PARENT)
-
-        self.Bind(wx.EVT_TREE_ITEM_ACTIVATED, self.OnItemActivated,
-                  self.dirtree)
-
-    def OnItemActivated(self, event):
-        currentItem = event.GetItem()
-        filename = self.dirtree.GetItemText(currentItem)
-        parentItem = self.dirtree.GetItemParent(currentItem)
-        d = self.dirtree.GetItemData(parentItem)
-        if isinstance(d, Directory):
-            filepath = os.path.join(d.directory, filename)
-        else:
-            return
-        if self.dirtree.ItemHasChildren(currentItem):
-            self.dirtree.SetRootDir(filepath)
-            return
-        (_, ext) = os.path.splitext(filename)
-        if ext == '.py':
-            dp.send(signal='frame.file_drop', filename=filepath)
-        else:
-            os.system("start " + filepath)
+        self.header = wx.StaticBitmap(self.panel)
+        self.header.SetBitmap(svg_to_bitmap(bsmedit_svg, 128, 128,  win=self))
+        szPanelAll.Add(self.header, 0, wx.EXPAND, 0)
 
-    def OnGotoHome(self, event):
-        root = self.dirtree.GetRootItem()
-        if not root:
-            return
-        d = self.dirtree.GetItemData(root)
-        if isinstance(d, Directory):
-            if d.directory == os.getcwd():
-                return
-        self.dirtree.SetRootDir(os.getcwd())
 
-    def OnGotoParent(self, event):
-        root = self.dirtree.GetRootItem()
-        if not root:
-            return
-        d = self.dirtree.GetItemData(root)
-        if isinstance(d, Directory):
-            path = os.path.abspath(os.path.join(d.directory, os.path.pardir))
-            if path == d.directory:
-                return
-            self.dirtree.SetRootDir(path)
+        szPanel = wx.BoxSizer(wx.VERTICAL)
+        szPanel.AddStretchSpacer(1)
+        MAX_SIZE = 300
+        caption = 'bsmedit %s' % (__version__)
+        self.stCaption = wx.StaticText(self.panel, wx.ID_ANY, caption)
+        self.stCaption.SetMaxSize((MAX_SIZE, -1))
+        self.stCaption.Wrap(MAX_SIZE)
+        self.stCaption.SetFont(wx.Font(16, 74, 90, 92, False, "Arial"))
 
+        szPanel.Add(self.stCaption, 0, wx.ALL | wx.EXPAND, 5)
 
-class MiscTools(object):
-    frame = None
+        strCopyright = f'(c) 2018-{datetime.datetime.now().year} Tianzhu Qiao. All rights reserved.'
+        self.stCopyright = wx.StaticText(self.panel, wx.ID_ANY, strCopyright)
+        self.stCopyright.SetMaxSize((MAX_SIZE, -1))
+        self.stCopyright.Wrap(MAX_SIZE)
+        self.stCopyright.SetFont(wx.Font(10, 74, 90, 90, False, "Arial"))
+        szPanel.Add(self.stCopyright, 0, wx.ALL | wx.EXPAND, 5)
 
-    @classmethod
-    def Initialize(cls, frame, **kwargs):
-        if cls.frame:
-            return
-        cls.frame = frame
-        if not frame:
-            return
+        build = wx.GetOsDescription() + '; wxWidgets ' + wx.version()
+        self.stBuild = wx.StaticText(self.panel, wx.ID_ANY, build)
+        self.stBuild.SetMaxSize((MAX_SIZE, -1))
+        self.stBuild.Wrap(MAX_SIZE)
+        self.stBuild.SetFont(wx.Font(10, 74, 90, 90, False, "Arial"))
+        szPanel.Add(self.stBuild, 0, wx.ALL | wx.EXPAND, 5)
+
+        stLine = wx.StaticLine(self.panel, style=wx.LI_HORIZONTAL)
+        szPanel.Add(stLine, 0, wx.EXPAND | wx.ALL, 0)
+        szPanel.AddStretchSpacer(1)
+
+        szPanelAll.Add(szPanel, 1, wx.EXPAND | wx.ALL, 0)
+
+        self.panel.SetSizer(szPanelAll)
+        self.panel.Layout()
+        szPanel.Fit(self.panel)
+
+        szAll.Add(self.panel, 1, wx.EXPAND | wx.ALL, 0)
+
+        btnsizer = wx.StdDialogButtonSizer()
+
+        self.btnOK = wx.Button(self, wx.ID_OK)
+        self.btnOK.SetDefault()
+        btnsizer.AddButton(self.btnOK)
+        btnsizer.Realize()
+
+        szAll.Add(btnsizer, 0, wx.ALIGN_RIGHT, 5)
 
-        active = kwargs.get('active', True)
-        direction = kwargs.get('direction', 'top')
-        # history panel
-        cls.panelHistory = HistoryPanel(frame)
-        dp.send(signal='frame.add_panel',
-                panel=cls.panelHistory,
-                title="History",
-                showhidemenu='View:Panels:Command History',
-                active=active,
-                direction=direction)
-        # help panel
-        cls.panelHelp = HelpPanel(frame)
-        dp.send(signal='frame.add_panel',
-                panel=cls.panelHelp,
-                title="Help",
-                target='History',
-                showhidemenu='View:Panels:Command Help',
-                active=active,
-                direction=direction)
-        # directory panel
-        cls.panelDir = DirPanel(frame)
-        dp.send(signal='frame.add_panel',
-                panel=cls.panelDir,
-                title="Browsing",
-                target="History",
-                showhidemenu='View:Panels:Browsing',
-                active=active,
-                direction=direction)
-
-        dp.connect(receiver=cls.Uninitialize, signal='frame.exit')
-
-    @classmethod
-    def Uninitialize(cls):
-        """destroy the module"""
-        pass
-
-
-def bsm_initialize(frame, **kwargs):
-    """module initialization"""
-    MiscTools.Initialize(frame, **kwargs)
+        self.SetSizer(szAll)
+        self.Layout()
+        szAll.Fit(self)
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/pymgr_helpers.py` & `bsmedit-3.2.9/bsmedit/bsm/pymgr_helpers.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/bsm/shell.py` & `bsmedit-3.2.9/bsmedit/bsm/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,180 +1,57 @@
 import os
 import sys
 import re
 import traceback
-import subprocess as sp
-import keyword
 import time
 import pydoc
+import glob
+import shlex
 import six.moves.builtins as __builtin__
 import six
 import wx
 import wx.py.shell as pyshell
 import wx.py.dispatcher as dp
 from wx import stc
 from wx.py.pseudo import PseudoFile
 from .debugger import EngineDebugger
 from ..version import __version__
+from .editor_base import EditorTheme, EditorFind
+from .shell_base import magic, aliasDict, sx
 
 
 # in linux, the multiprocessing/process.py/_bootstrap will call
 # sys.stdin.close(), which is missing in wx.py.pseudo.PseudoFile
 def PseudoFile_close(self):
     pass
 
-
 PseudoFile.close = PseudoFile_close
 
-aliasDict = {}
-
-
-def magicSingle(command):
-    if command == '':  # Pass if command is blank
-        return command
-
-    first_space = command.find(' ')
-
-    if command[0] == ' ':  # Pass if command begins with a space
-        pass
-    elif command[0] == '?':  # Do help if starts with ?
-        command = 'help(' + command[1:] + ')'
-    elif command[0] == '!':  # Use os.system if starts with !
-        command = 'sx("' + command[1:] + '")'
-    elif command in ('ls', 'pwd'):
-        # automatically use ls and pwd with no arguments
-        command = command + '()'
-    elif command[:3] in ('ls ', 'cd '):
-        # when using the 'ls ' or 'cd ' constructs, fill in both parentheses and quotes
-        command = command[:2] + '("' + command[3:] + '")'
-    elif command[:5] in ('help ', ):
-        command = command[:4] + '("' + command[5:] + '")'
-    elif command[:6] == 'close ':
-        arg = command[6:]
-        if arg.strip() == 'all':
-            # when using the close', fill in both parentheses and quotes
-            command = command[:5] + '("' + command[6:] + '")'
-    elif command[:5] == 'clear':
-        command = command[:5] + '()'
-    elif command[:5] == 'alias':
-        c = command[5:].lstrip().split(' ')
-        if len(c) < 2:
-            # delete the alias if exists
-            if len(c) == 1:
-                aliasDict.pop(c[0], None)
-            command = ''
-        else:
-            n, v = c[0], ' '.join(c[1:])
-            aliasDict[n] = v
-            command = ''
-    elif command.split(' ')[0] in six.iterkeys(aliasDict):
-        c = command.split(' ')
-        if len(c) < 2:
-            command = 'sx("' + aliasDict[c[0]] + '")'
-        else:
-            command = 'sx("' + aliasDict[c[0]] + ' ' + ' '.join(c[1:]) + '")'
-    elif first_space != -1:
-        # if there is at least one space, add parentheses at beginning and end
-        cmds = command.split(' ')
-        if len(cmds) > 1:
-            wd1 = cmds[0]
-            wd2 = cmds[1]
-            i = 1
-            while wd2 == '':
-                i += 1
-                if len(cmds) == i:
-                    break
-                wd2 = cmds[i]
-            if wd2 == '':
-                return command
-            if (wd1[0].isalpha() or wd1[0] == '_') and (wd2[0].isalnum() or\
-                    (wd2[0] in """."'_""")) and \
-                    not keyword.iskeyword(wd1) and not keyword.iskeyword(wd2):
-                if wd1.replace('.', '').replace('_', '').isalnum():
-                    # add parentheses where the first space was and at the end... hooray!
-                    command = wd1 + '(' + command[(first_space + 1):] + ')'
-    return command
-
 
 def _help(command):
     try:
-        print(pydoc.plain(pydoc.render_doc(str(command), "Help on %s")))
-    except:
-        print('No help found on "%s"' % command)
-
-
-def magic(command):
-    continuations = wx.py.parse.testForContinuations(command)
-    if len(continuations) == 2:  # Error case...
-        return command
-    elif len(continuations) == 4:
-        stringContinuationList, indentationBlockList, \
-        lineContinuationList, parentheticalContinuationList = continuations
-
-    commandList = []
-    firstLine = True
-    for i in command.split('\n'):
-        if firstLine:
-            commandList.append(magicSingle(i))
-        elif stringContinuationList.pop(0) is False and \
-              indentationBlockList.pop(0) is False and \
-              lineContinuationList.pop(0) is False and \
-              parentheticalContinuationList.pop(0) is False:
-            commandList.append(magicSingle(
-                i))  # unless this is in a larger expression, use magic
+        if isinstance(command, str):
+            print(pydoc.plain(pydoc.render_doc(command, "Help on %s")))
         else:
-            commandList.append(i)
-
-        firstLine = False
-
-    return '\n'.join(commandList)
-
-
-def sx(cmd, *args, **kwds):
-    wait = True
-    # append '&' to capture the output
-    if cmd[-1] == '&':
-        wait = False
-        cmd = cmd[0:-1]
-    startupinfo = None
-    if wx.Platform == '__WXMSW__':
-        startupinfo = sp.STARTUPINFO()
-        startupinfo.dwFlags |= sp.STARTF_USESHOWWINDOW
-    # try the standalone command first
-    try:
-        if wait:
-            p = sp.Popen(cmd.split(' '),
-                         startupinfo=startupinfo,
-                         stdout=sp.PIPE,
-                         stderr=sp.PIPE)
-            dp.send('shell.write_out', text=p.stdout.read().decode())
-        else:
-            p = sp.Popen(cmd.split(' '), startupinfo=startupinfo)
-        return
+            print(command.__doc__)
     except:
-        traceback.print_exc(file=sys.stdout)
-    # try the shell command
-    try:
-        if wait:
-            p = sp.Popen(cmd.split(' '),
-                         startupinfo=startupinfo,
-                         shell=True,
-                         stdout=sp.PIPE,
-                         stderr=sp.PIPE)
-            dp.send('shell.write_out', text=p.stdout.read().decode())
-        else:
-            p = sp.Popen(cmd.split(' '), startupinfo=startupinfo, shell=True)
-        return
-    except:
-        traceback.print_exc(file=sys.stdout)
+        print(f'No help found on "{command}"')
 
+def _doc(command):
+    if isinstance(command, str):
+        dp.send('help.show', command=command)
+    else:
+        _help(command)
 
+@EditorFind
+@EditorTheme
 class Shell(pyshell.Shell):
     ID_COPY_PLUS = wx.NewId()
     ID_PASTE_PLUS = wx.NewId()
+    ID_WRAP_MODE = wx.NewIdRef()
 
     def __init__(self,
                  parent,
                  id=-1,
                  pos=wx.DefaultPosition,
                  size=wx.DefaultSize,
                  style=wx.CLIP_CHILDREN,
@@ -188,38 +65,50 @@
         # variables used in push, which may be called by
         # wx.py.shell.Shell.__init__ when execStartupScript is True
         self.enable_debugger = False
         self.silent = True
         pyshell.Shell.__init__(self, parent, id, pos, size, style, introText,
                                locals, InterpClass, startupScript,
                                execStartupScript, useStockId=False, *args, **kwds)
-        wx.CallAfter(self.redirectStdout, True)
-        wx.CallAfter(self.redirectStderr, True)
-        #self.redirectStdout(True)
-        #self.redirectStderr(True)
+
+        theme = 'solarized-dark'
+        resp = dp.send('frame.get_config', group='shell', key='theme')
+        if resp and resp[0][1] is not None:
+            theme = resp[0][1]
+        self.SetupColor(theme)
+        c = self.GetThemeColor()
+        self.SetCaretForeground(c['emphasized'])
+        self.SetCaretStyle(wx.stc.STC_CARETSTYLE_BLOCK)
         # the default sx function (!cmd to run external command) does not work
         # on windows
         __builtin__.sx = sx
         self.callTipInsert = False
         self.searchHistory = True
         self.silent = False
         self.autoIndent = True
         self.running = False
-        self.debugger = EngineDebugger()
+        self.debugger = EngineDebugger(pyshell.USE_MAGIC)
         self.LoadHistory()
         self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
         self.Bind(wx.EVT_LEFT_DCLICK, self.OnLeftDClick)
+        self.Bind(stc.EVT_STC_DO_DROP, self.OnDoDrop)
+        self.Bind(stc.EVT_STC_START_DRAG, self.OnStartDrag)
+        self.Bind(wx.EVT_MENU, self.OnWrapMode, self.ID_WRAP_MODE)
+
         self.interp.locals['clear'] = self.clear
         self.interp.locals['help'] = _help
+        self.interp.locals['doc'] = _doc
         self.interp.locals['on'] = True
         self.interp.locals['off'] = False
         dp.connect(self.writeOut, 'shell.write_out')
         dp.connect(self.runCommand, 'shell.run')
         dp.connect(self.debugPrompt, 'shell.prompt')
         dp.connect(self.addHistory, 'shell.add_to_history')
+        dp.connect(self.clearHistory, 'shell.clear_history')
+        dp.connect(self.deleteHistory, 'shell.delete_history')
         dp.connect(self.IsDebuggerOn, 'debugger.debugging')
         dp.connect(self.getAutoCompleteList, 'shell.auto_complete_list')
         dp.connect(self.getAutoCompleteKeys, 'shell.auto_complete_keys')
         dp.connect(self.getAutoCallTip, 'shell.auto_call_tip')
         dp.connect(self.OnActivatePanel, 'frame.activate_panel')
         dp.connect(self.OnActivate, 'frame.activate')
         dp.connect(self.OnFrameClosing, 'frame.closing')
@@ -234,126 +123,67 @@
             self.CmdKeyAssign(ord('E'), wx.stc.STC_SCMOD_META, wx.stc.STC_CMD_LINEEND)
             self.CmdKeyAssign(ord('A'), wx.stc.STC_SCMOD_META, wx.stc.STC_CMD_VCHOME)
 
         self.Bind(wx.EVT_UPDATE_UI, lambda evt: evt.Enable(True), id=self.ID_CLEAR)
         self.Bind(wx.EVT_MENU, lambda evt: self.clear(), id=self.ID_CLEAR)
 
         # find dialog
-        eid = wx.NewId()
-        self.Bind(wx.EVT_MENU, self.OnShowFindReplace, id=eid)
-        accel_tbl = wx.AcceleratorTable([(wx.ACCEL_CTRL, ord('F'), eid)])
+        self.SetupFind()
+        # disable replace
+        self.findDialogStyle = 0
+
+        eid_ctl_c = wx.NewIdRef()
+        self.Bind(wx.EVT_MENU, self.OnCtrlC, id=eid_ctl_c)
+        accel_tbl = wx.AcceleratorTable([(wx.ACCEL_CTRL, ord('F'), self.ID_FIND_REPLACE),
+                                         (wx.ACCEL_RAW_CTRL, ord('C'), eid_ctl_c)])
         self.SetAcceleratorTable(accel_tbl)
-        self.findDialog = None
-        self.findStr = ""
-        self.findFlags = 1
-        self.stcFindFlags = 0
 
+        self.LoadConfig()
+    def SetConfig(self):
+        dp.send('frame.set_config', group='shell', wrap=self.GetWrapMode() != wx.stc.STC_WRAP_NONE)
+
+    def LoadConfig(self):
+        resp = dp.send('frame.get_config', group='shell', key='wrap')
+        if resp and resp[0][1] is not None:
+            if resp[0][1]:
+                self.SetWrapMode(wx.stc.STC_WRAP_WORD)
+            else:
+                self.SetWrapMode(wx.stc.STC_WRAP_NONE)
     def clear(self):
         super().clear()
         self.prompt()
 
-    def OnShowFindReplace(self, event):
-        """Find and Replace dialog and action."""
-        # find string
-        findStr = self.GetSelectedText()
-        if findStr and self.findDialog:
-            self.findDialog.Destroy()
-            self.findDialog = None
-        # dialog already open, if yes give focus
-        if self.findDialog:
-            self.findDialog.Show(1)
-            self.findDialog.Raise()
-            return
-        if not findStr:
-            findStr = self.findStr
-        # find data
-        data = wx.FindReplaceData(self.findFlags)
-        data.SetFindString(findStr)
-        # dialog
-        self.findDialog = wx.FindReplaceDialog(
-            self, data, 'Find')
-        # bind the event to the dialog, see the example in wxPython demo
-        self.findDialog.Bind(wx.EVT_FIND, self.OnFind)
-        self.findDialog.Bind(wx.EVT_FIND_NEXT, self.OnFind)
-        self.findDialog.Bind(wx.EVT_FIND_CLOSE, self.OnFindClose)
-        self.findDialog.Show(1)
-        self.findDialog.data = data  # save a reference to it...
-
-    def message(self, text):
-        """show the message on statusbar"""
-        dp.send('frame.show_status_text', text=text)
-
-    def _find_text(self, minPos, maxPos, text, flags=0):
-        position = self.FindText(minPos, maxPos, text, flags)
-        if isinstance(position, tuple):
-            position = position[0] # wx ver 4.1.0 returns (start, end)
-        return position
-
-    def doFind(self, strFind, forward=True):
-        """search the string"""
-        current = self.GetCurrentPos()
-        position = -1
-        if forward:
-            position = self._find_text(current, len(self.GetText()),
-                                       strFind, self.stcFindFlags)
-            if position == -1:
-                # wrap around
-                position = self._find_text(0, current + len(strFind), strFind,
-                                           self.stcFindFlags)
+    def OnCtrlC(self, event):
+        if self.CanCopy():
+            self.Copy()
         else:
-            position = self._find_text(current - len(strFind), 0, strFind,
-                                       self.stcFindFlags)
-            if position == -1:
-                # wrap around
-                position = self._find_text(len(self.GetText()), current,
-                                           strFind, self.stcFindFlags)
-
-        # not found the target, do not change the current position
-        if position == -1:
-            self.message("'%s' not found!" % strFind)
-            position = current
-            strFind = """"""
-        self.GotoPos(position)
-        self.SetSelection(position, position + len(strFind))
-        return position
-
-    def OnFind(self, event):
-        """search the string"""
-        self.findStr = event.GetFindString()
-        self.findFlags = event.GetFlags()
-        flags = 0
-        if wx.FR_WHOLEWORD & self.findFlags:
-            flags |= stc.STC_FIND_WHOLEWORD
-        if wx.FR_MATCHCASE & self.findFlags:
-            flags |= stc.STC_FIND_MATCHCASE
-        self.stcFindFlags = flags
-        return self.doFind(self.findStr, wx.FR_DOWN & self.findFlags)
-
-    def OnFindClose(self, event):
-        """close find & replace dialog"""
-        event.GetDialog().Destroy()
+            self.interp.more = False
+            endpos = self.GetTextLength()
+            self.GotoPos(endpos)
+            self.push('', history=False)
 
     def Destroy(self):
         self.debugger.release()
         # save command history
         dp.send('frame.set_config', group='shell', history=self.history)
         dp.send('frame.set_config', group='shell', alias=aliasDict)
+        dp.send('frame.set_config', group='shell', zoom=self.GetZoom())
 
         dp.disconnect(self.writeOut, 'shell.write_out')
         dp.disconnect(self.runCommand, 'shell.run')
         dp.disconnect(self.debugPrompt, 'shell.prompt')
         dp.disconnect(self.addHistory, 'shell.add_to_history')
         dp.disconnect(self.IsDebuggerOn, 'debugger.debugging')
         dp.disconnect(self.getAutoCompleteList, 'shell.auto_complete_list')
         dp.disconnect(self.getAutoCompleteKeys, 'shell.auto_complete_keys')
         dp.disconnect(self.getAutoCallTip, 'shell.auto_call_tip')
         dp.disconnect(self.OnActivatePanel, 'frame.activate_panel')
         dp.disconnect(self.OnActivate, 'frame.activate')
         dp.disconnect(self.OnFrameClosing, 'frame.closing')
-        super(Shell, self).Destroy()
+        super().Destroy()
 
     def OnFrameClosing(self, event):
         """the frame is exiting"""
         if self.IsDebuggerOn() and event.CanVeto():
             # stop closing if the debugger is running, otherwise it may crash
             # as some events (e.g., ID_DEBUG_SCRIPT in editor) may be
             # called after some window (e.g., editor) has been destroyed.
@@ -395,15 +225,16 @@
                     return None
 
     def Paste(self):
         """Replace selection with clipboard contents."""
         if self.CanPaste() and wx.TheClipboard.Open():
             ps2 = str(sys.ps2)
             # on mac 11.4, it always return false
-            if True:#wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_TEXT)):
+            if wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_TEXT)) or\
+               wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_UNICODETEXT)):
                 data = wx.TextDataObject()
                 if wx.TheClipboard.GetData(data):
                     self.ReplaceSelection('')
                     command = data.GetText()
                     command = command.rstrip()
                     command = self.fixLineEndings(command)
                     command = self.lstripPrompt(text=command)
@@ -413,15 +244,16 @@
                     self.write(command)
             wx.TheClipboard.Close()
 
     def PasteAndRun(self):
         """Replace selection with clipboard contents, run commands."""
         text = ''
         if wx.TheClipboard.Open():
-            if True:#wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_TEXT)):
+            if wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_TEXT)) or\
+               wx.TheClipboard.IsSupported(wx.DataFormat(wx.DF_UNICODETEXT)):
                 data = wx.TextDataObject()
                 if wx.TheClipboard.GetData(data):
                     text = data.GetText()
             wx.TheClipboard.Close()
         if text:
             self.Execute(text)
 
@@ -433,15 +265,49 @@
         kwds.pop('sender', None)
         kwds.pop('signal', None)
         try:
             cmd = wx.py.introspect.getRoot(command, '.')
             self.evaluate(cmd)
         except:
             pass
-        return self.interp.getAutoCompleteList(command, *args, **kwds)
+        cmp = self.interp.getAutoCompleteList(command, *args, **kwds)
+        part = command[command.rfind('.') + 1:]
+        if part:
+            part = part.lower()
+            cmp = [c for c in cmp if c.lower().startswith(part)]
+        return cmp
+
+    def getPathList(self, path=None, prefix='', files=True, folders=True):
+        paths = []
+        if path is None:
+            path = os.getcwd()
+        def _getPathList(pattern):
+            # get folders or files
+            f = glob.glob(pattern)
+            # remove common "path"
+            f = [os.path.relpath(folder, path) for folder in f]
+            # check if start with prefix
+            f = [folder for folder in f if folder.lower().startswith(prefix.lower())]
+            # replace ' ' with '\ ' or put the path in quotes to indicate it is a
+            # space in path not in command
+            if wx.Platform == '__WXMSW__':
+                f = [ f'"{p}"' if ' ' in p else p for p in f]
+            else:
+                f = [p.replace(' ', r'\ ') for p in f]
+            return f
+
+        if folders:
+            f = _getPathList(os.path.join(path, '*/'))
+            f = [folder + '/' for folder in f]
+            paths += sorted(f, key=str.casefold)
+        if files:
+            f = _getPathList(os.path.join(path, '*.*'))
+            paths += sorted(f, key=str.casefold)
+
+        return paths
 
     def getAutoCallTip(self, command, *args, **kwds):
         # remove additional key from wx.py.dispatcher.send
         kwds.pop('sender', None)
         kwds.pop('signal', None)
         return self.interp.getCallTip(command, *args, **kwds)
 
@@ -454,80 +320,103 @@
                 if not (c.isalnum() or c in ('_', '.')):
                     command = command[-i:]
                     break
             cmd = wx.py.introspect.getRoot(command, '.')
             self.evaluate(cmd)
         except:
             pass
-        super(Shell, self).autoCompleteShow(command, offset)
+        super().autoCompleteShow(command, offset)
 
     def IsDebuggerOn(self):
         """check if the debugger is on"""
         if not self.debugger:
             return False
         return self.enable_debugger
 
-    def SetSelection(self, start, end):
-        self.SetSelectionStart(start)
-        self.SetSelectionEnd(end)
-        if end < start:
-            self.SetAnchor(start)
+    def IsDebuggerPaused(self):
+        return self.IsDebuggerOn() and self.debugger._paused
+
+    def SetSelection(self, from_, to_):
+        self.SetSelectionStart(from_)
+        self.SetSelectionEnd(to_)
+        if to_ < from_:
+            self.SetAnchor(from_)
 
     def LoadHistory(self):
         self.clearHistory()
         resp = dp.send('frame.get_config', group='shell', key='history')
         if resp and resp[0][1]:
             self.history = resp[0][1]
         resp = dp.send('frame.get_config', group='shell', key='alias')
         if resp and resp[0][1]:
             aliasDict.update(resp[0][1])
+        resp = dp.send('frame.get_config', group='shell', key='zoom')
+        if resp and resp[0][1]:
+            try:
+                self.SetZoom(int(resp[0][1]))
+            except:
+                pass
 
     def OnKillFocus(self, event):
         if self.CallTipActive():
             self.CallTipCancel()
         if self.AutoCompActive():
-            wx.CallAfter(self.AutoCompCancel)
+            self.AutoCompCancel()
         event.Skip()
 
     def OnActivate(self, activate):
         # not work on mac
         if wx.Platform == '__WXMAC__':
             return
 
         if self.AutoCompActive():
-            wx.CallAfter(self.AutoCompCancel)
+            self.AutoCompCancel()
 
     def OnActivatePanel(self, pane):
         if pane != self:
             if self.AutoCompActive():
-                wx.CallAfter(self.AutoCompCancel)
+                self.AutoCompCancel()
 
-    def OnUpdateUI(self, evt):
-        eid = evt.GetId()
+    def OnUpdateUI(self, event):
+        eid = event.GetId()
         if eid in (wx.ID_CUT, wx.ID_CLEAR):
-            evt.Enable(self.CanCut())
+            event.Enable(self.CanCut())
         elif eid in (wx.ID_COPY, self.ID_COPY_PLUS):
-            evt.Enable(self.CanCopy())
+            event.Enable(self.CanCopy())
         elif eid in (wx.ID_PASTE, self.ID_PASTE_PLUS):
-            evt.Enable(self.CanPaste())
+            event.Enable(self.CanPaste())
         elif eid == wx.ID_UNDO:
-            evt.Enable(self.CanUndo())
+            event.Enable(self.CanUndo())
         elif eid == wx.ID_REDO:
-            evt.Enable(self.CanRedo())
+            event.Enable(self.CanRedo())
         # update the caret position so that it is always in valid area
         self.UpdateCaretPos()
-        super(Shell, self).OnUpdateUI(evt)
+        super().OnUpdateUI(event)
 
     def UpdateCaretPos(self):
         # when editing the command, do not allow moving the caret to
         # readonly area
         if not self.CanEdit() and \
                 (self.GetCurrentLine() == self.LineFromPosition(self.promptPosEnd)):
             self.GotoPos(self.promptPosEnd)
 
+    def GetContextMenu(self):
+        menu = super().GetContextMenu()
+        menu.AppendSeparator()
+        menu.AppendCheckItem(self.ID_WRAP_MODE, 'Word wrap')
+        menu.Check(self.ID_WRAP_MODE, self.GetWrapMode() != wx.stc.STC_WRAP_NONE)
+        return menu
+
+    def OnWrapMode(self, event):
+        if self.GetWrapMode() == wx.stc.STC_WRAP_NONE:
+            self.SetWrapMode(wx.stc.STC_WRAP_WORD)
+        else:
+            self.SetWrapMode(wx.stc.STC_WRAP_NONE)
+        self.SetConfig()
+
     def OnKeyDown(self, event):
         """Key down event handler."""
         key = event.GetKeyCode()
         # If the auto-complete window is up let it do its thing.
         if self.AutoCompActive():
             event.Skip()
             return
@@ -554,36 +443,85 @@
         elif canEdit and not self.more and (
                 not shiftDown) and key == wx.WXK_DOWN:
             # Replace with the next command from the history buffer.
             self.GoToHistory(False)
         elif canEdit and (not shiftDown) and key == wx.WXK_TAB:
             # show auto-complete list with TAB
             # first try to get the autocompletelist from the package
-            cmd = self.getCommand()
+            cmd = self.getCommandLeft(rstrip=False)
             k = self.getAutoCompleteList(cmd)
-            cmd = cmd[cmd.rfind('.') + 1:]
-            # if failed, search the locals()
+            lengthEntered = 0
+            if k:
+                lengthEntered = len(cmd[cmd.rfind('.') + 1:])
+            sep = ' '
             if not k:
+                # check path
+                # use shlex.split to handle cases like:
+                # '!ls /Users/my\ folder'
+                try:
+                    cmds = shlex.split(cmd)
+                    cmd_main = cmds[0]
+                    prefix = cmds[-1] if len(cmds) > 1 else ''
+                    path, prefix = os.path.split(prefix)
+                    if cmd_main in ['cd', '!cd', '!rmdir', '!mkdir']:
+                        k = self.getPathList(path=path, prefix=prefix, files=False)
+                    elif cmd_main in ['ls', '!ls', '!less', '!more', '!cp', '!mv',\
+                                      '!rm', '!gvim']:
+                        k = self.getPathList(path=path, prefix=prefix)
+                    lengthEntered = len(prefix)
+                    if ' ' in prefix:
+                        if wx.Platform == '__WXMSW__':
+                            lengthEntered += 2
+                        else:
+                            lengthEntered += prefix.count(' ')
+                    # use a character that will not appear in path
+                    if k:
+                        sep = '`'
+                except:
+                    pass
+
+            # if failed, search the locals()
+            if not k and cmd:
                 for i in six.moves.range(len(cmd) - 1, -1, -1):
                     if cmd[i].isalnum() or cmd[i] == '_':
                         continue
+                    if cmd[i] in ['.']:
+                        # invalid
+                        cmd = ''
+                        break
                     cmd = cmd[i + 1:]
                     break
-                k = six.iterkeys(self.interp.locals)
-                k = [s for s in k if s.startswith(cmd)]
-                k.sort()
+                if cmd:
+                    k = six.iterkeys(self.interp.locals)
+                    k = [s for s in k if s.startswith(cmd)]
+                    k.sort()
+
             if k:
+                self.AutoCompSetSeparator(ord(sep))
                 self.AutoCompSetAutoHide(self.autoCompleteAutoHide)
                 self.AutoCompSetIgnoreCase(self.autoCompleteCaseInsensitive)
-                options = ' '.join(k)
-                self.AutoCompShow(len(cmd), options)
+                options = sep.join(k)
+                lengthEntered = len(cmd) if all(item.lower().startswith(cmd.lower()) for item in k) else lengthEntered
+                self.AutoCompShow(lengthEntered, options)
+                self.AutoCompSetSeparator(ord(' '))
             return
         else:
             self.searchHistory = True
-            super(Shell, self).OnKeyDown(event)
+            # Reset the history position.
+            self.historyIndex = -1
+            super().OnKeyDown(event)
+
+    def getCommandLeft(self, rstrip=True):
+        # get the command up to the cursor
+        startpos = self.promptPosEnd
+        endpos = self.GetCurrentPos()
+        command = self.GetTextRange(startpos, endpos)
+        if rstrip:
+            command = command.rstrip()
+        return command
 
     def OnLeftDClick(self, event):
         line_num = self.GetCurrentLine()
         line = self.GetLine(line_num)
         filepath = re.findall('[Ff]ile [^,]+,', line)
         if filepath:
             path = (filepath[0])[6:-2]
@@ -598,34 +536,38 @@
                     lineno=linenum)
         event.Skip()
 
     def GoToHistory(self, up=True):
         """Search up the history buffer for the text in front of the cursor."""
         if not self.CanEdit():
             return
+        startpos = self.promptPosEnd
+        endpos = self.GetTextLength()
+        fullText = self.GetTextRange(startpos, endpos)
         startpos = self.GetCurrentPos()
         # The text up to the cursor is what we search for.
         numCharsAfterCursor = self.GetTextLength() - startpos
-        searchText = self.getCommand(rstrip=False)
+        searchText = fullText
         if numCharsAfterCursor > 0:
             searchText = searchText[:-numCharsAfterCursor]
-        if not searchText or self.searchHistory == False:
+        if not searchText or not self.searchHistory:
             self.OnHistoryReplace(step=up * 2 - 1)
             self.searchHistory = False
             return
         # Search upwards from the current history position and loop
         # back to the beginning if we don't find anything.
         if up:
             searchOrder = six.moves.range(self.historyIndex + 1,
                                           len(self.history))
         else:
             searchOrder = six.moves.range(self.historyIndex - 1, -1, -1)
         for i in searchOrder:
             command = self.history[i]
-            if command[:len(searchText)] == searchText:
+            if command[:len(searchText)] == searchText and fullText != command:
+                # ignore the exact same command
                 # Replace the current selection with the one we found.
                 endpos = self.GetTextLength()
                 self.SetSelection(startpos, endpos)
                 self.ReplaceSelection(command[len(searchText):])
                 endpos = self.GetCurrentPos()
                 self.SetSelection(endpos, startpos)
                 # We've now warped into middle of the history.
@@ -634,22 +576,25 @@
             self.historyIndex = i
 
     def writeOut(self, text):
         """Replacement for stdout."""
         # only output the text when it is not silent
         try:
             if not self.silent:
-                wx.CallAfter(self.AutoCompCancel)
+                # not use wx.CallAfter in this function, otherwise it may
+                # crash when close the app (e.g., shell is destroyed when
+                # wx.CallAfter function is called
+                self.AutoCompCancel()
                 # move the cursor to the end to protect the readonly section
                 endpos = self.GetTextLength()
                 # remember the current position (relative to end)
                 offset = endpos - self.GetCurrentPos()
                 if not self.CanEdit():
                     self.SetCurrentPos(endpos)
-                if not self.waiting:
+                if not self.waiting:# or self.IsDebuggerPaused():
                     # if the shell is in idle status, output the text right before the prompt
                     self.SetCurrentPos(self.promptPosStart)
                     self.write(text)
                     self.promptPosStart += self.GetTextLength() - endpos
                     self.promptPosEnd += self.GetTextLength() - endpos
                 else:
                     if self.GetCurrentLine() \
@@ -676,15 +621,31 @@
         self.writeOut(text)
 
     def addHistory(self, command):
         # override the parent function to add time-stamp.
         stamp = time.strftime('#bsm#%Y/%m/%d')
         if stamp not in self.history:
             self.history.insert(0, stamp)
-        super(Shell, self).addHistory(command)
+        super().addHistory(command)
+
+    def deleteHistory(self, command, timestamp="", index=-1):
+        for i in six.moves.range(len(self.history) - 1, -1, -1):
+            if self.history[i] == timestamp:
+                if command == timestamp:
+                    # delete folder
+                    m = 1
+                    while(i-m>=0 and not self.history[i-m].startswith('#bsm#')):
+                        m += 1
+                    del self.history[i-m+1:i]
+                    break
+                else:
+                    idx = i-index-1
+                    if idx>=0 and self.history[idx] == command:
+                        del self.history[idx]
+                    break
 
     def runCommand(self,
                    command,
                    prompt=True,
                    verbose=True,
                    debug=False,
                    history=True):
@@ -709,54 +670,74 @@
         self.push(command, not prompt, history)
 
         # retrieve the typed command
         if not self.more and command_typed:
             self.write(command_typed)
         self.autoIndent = True
 
+    def push_multiple_line(self, command, silent=False, history=True):
+        commands = command.splitlines(keepends=False)
+        if command.endswith('\n'):
+            # keep the newline at the end, so an empty line will finish
+            # the statement
+            commands.append('')
+        if not commands:
+            # run the empty command (e.g., to start the prompt in a new line)
+            commands = ['']
+
+        # run the command line by line
+        cmd_raw = []
+        for idx, cmd in enumerate(commands):
+            if idx != len(commands) -1 and not cmd and cmd_raw:
+                p = cmd_raw[-1]
+                cmd = p[:len(p) - len(p.lstrip())]
+            cmd_raw.append(cmd)
+            if pyshell.USE_MAGIC:
+                cmd = magic(cmd)
+            if len(cmd) > 1 and cmd[-1] == ';':
+                self.silent = True
+            self.waiting = True
+            self.lastUpdate = None
+            try:
+                if self.enable_debugger:
+                    self.debugger.reset()
+                    sys.settrace(self.debugger)
+                self.more = self.interp.push(cmd)
+            except:
+                traceback.print_exc(file=sys.stdout)
+            finally:
+                # make sure debugger.ended is always sent; more does not hurt
+                if self.enable_debugger:
+                    dp.send('debugger.ended')
+                    self.debugger.reset()
+                    self.enable_debugger = False
+
+            sys.settrace(None)
+            self.lastUpdate = None
+            self.waiting = False
+            self.silent = False
+            if not self.more and history:
+                # finished a statement, add it to history
+                self.addHistory('\n'.join(cmd_raw))
+                cmd_raw = []
+        if not silent:
+            self.prompt()
+
     def push(self, command, silent=False, history=True):
         """Send command to the interpreter for execution."""
         self.running = True
         if not silent:
             self.write(os.linesep)
         # push to the debugger
         if self.waiting and self.IsDebuggerOn():
             self.debugger.push_line(command)
             return
-        # DNM
-        cmd_raw = command
-        if pyshell.USE_MAGIC:
-            command = magic(command)
-        if len(command) > 1 and command[-1] == ';':
-            self.silent = True
 
-        self.waiting = True
-        self.lastUpdate = None
-        try:
-            if self.enable_debugger:
-                self.debugger.reset()
-                sys.settrace(self.debugger)
-            self.more = self.interp.push(command)
-        except:
-            traceback.print_exc(file=sys.stdout)
-        finally:
-            # make sure debugger.ended is always sent; more does not hurt
-            if self.enable_debugger:
-                dp.send('debugger.ended')
-                self.debugger.reset()
-                self.enable_debugger = False
-
-        sys.settrace(None)
-        self.lastUpdate = None
-        self.waiting = False
-        self.silent = False
-        if not self.more and history:
-            self.addHistory(cmd_raw)
-        if not silent:
-            self.prompt()
+        # DNM
+        self.push_multiple_line(command, silent=silent, history=history)
         self.running = False
 
     def lstripPrompt(self, text):
         """Return text without a leading prompt."""
         ps = [str(sys.ps1), str(sys.ps2), str(sys.ps3), str("K>> ")]
         # Strip the prompt off the front of text.
         for p in ps:
@@ -899,14 +880,15 @@
                     # value.
                     command = '\n'
                 self.reader.input = command
                 self.write(os.linesep)
             else:
                 self.push(command)
                 wx.CallAfter(self.EnsureCaretVisible)
+                wx.CallAfter(self.SetFocus)
         # Or replace the current command with the other command.
         else:
             # If the line contains a command (even an invalid one).
             if self.getCommand(rstrip=False):
                 command = self.getMultilineCommand()
                 self.clearCommand()
                 self.write(command)
@@ -916,34 +898,62 @@
                 self.SetAnchor(thepos)
 
     def setStyles(self, faces):
         super().setStyles(faces)
         self.StyleSetSpec(stc.STC_STYLE_LINENUMBER,
                           'fore:#3C3C43,back:#F2F2F7')
 
+    def OnStartDrag(self, event):
+        event.SetText('')
+
+    def OnDoDrop(self, event):
+        allow = self.CanEdit() and (event.GetPosition() >= self.promptPosEnd)
+        if allow:
+            self.InsertText(event.GetPosition(), event.GetText())
+        event.SetText('')
+
     @classmethod
     def Initialize(cls, frame, **kwargs):
         cls.frame = frame
+        dp.connect(receiver=cls.initialized, signal='frame.initialized')
         dp.connect(receiver=cls.Uninitialize, signal='frame.exit')
+        cls.debug = kwargs.get('debug', False)
         ns = {}
         ns['wx'] = wx
         ns['app'] = wx.GetApp()
         ns['frame'] = cls.frame
         intro = 'Welcome To bsmedit ' + __version__
         cls.panelShell = Shell(cls.frame, introText=intro, locals=ns)
         active = kwargs.get('active', True)
         direction = kwargs.get('direction', 'top')
         dp.send(signal="frame.add_panel",
                 panel=cls.panelShell,
                 active=active,
                 title="Shell",
-                showhidemenu="View:Panels:Console",
                 direction=direction)
 
     @classmethod
+    def initialized(cls):
+        if cls.panelShell and not cls.debug:
+            # not redirect if in debug mode
+            redirect = True
+            resp = dp.send('frame.get_config', group='shell', key='redirect_stdout')
+            if resp and resp[0][1] is not None:
+                redirect = resp[0][1]
+            cls.panelShell.redirectStdout(redirect)
+
+            redirect = True
+            resp = dp.send('frame.get_config', group='shell', key='redirect_stderr')
+            if resp and resp[0][1] is not None:
+                redirect = resp[0][1]
+            cls.panelShell.redirectStderr(redirect)
+
+    @classmethod
     def Uninitialize(cls):
         if cls.panelShell:
+            cls.panelShell.redirectStdout(False)
+            cls.panelShell.redirectStderr(False)
             dp.send('frame.delete_panel', panel=cls.panelShell)
 
 
 def bsm_initialize(frame, **kwargs):
     Shell.Initialize(frame, **kwargs)
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/sim.py` & `bsmedit-3.2.9/bsmedit/bsm/sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,35 @@
 import time
 import traceback
 import sys
 import six.moves.queue as Queue
 import six
 import wx
 import wx.py.dispatcher as dp
-import wx.lib.agw.aui as aui
+from ..aui import aui
 from ..auibarpopup import AuiToolBarPopupArt
 from . import graph
-from .bsmxpm import module_xpm, switch_xpm, in_xpm, out_xpm, inout_xpm,\
-                    module_grey_xpm, switch_grey_xpm, in_grey_xpm,\
-                    out_grey_xpm, inout_grey_xpm, step_svg, step_grey_svg, run_svg, run_grey_svg, \
-                    pause_svg, pause_grey_svg, setting_xpm, radio_disabled_svg, \
+from .bsmxpm import module_svg, signal_svg, input_svg, output_svg, inout_svg,\
+                    step_svg, step_grey_svg, run_svg, run_grey_svg, \
+                    pause_svg, pause_grey_svg, setting_svg, radio_disabled_svg, \
                     radio_activated_svg, radio_checked_svg, radio_unchecked_svg
 from .simprocess import sim_process, SC_OBJ_UNKNOWN, SC_OBJ_SIGNAL, SC_OBJ_INPUT,\
                         SC_OBJ_OUTPUT, SC_OBJ_INOUT, SC_OBJ_CLOCK, SC_OBJ_XSC_PROP,\
                         SC_OBJ_XSC_ARRAY_ITEM, SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY
 from .. import propgrid as pg
 from .pymgr_helpers import Gcm
 from .autocomplete import AutocompleteTextCtrl
 from .utility import MakeBitmap, FastLoadTreeCtrl, PopupMenu
 from .. import to_byte
 from .utility import svg_to_bitmap
 
 Gcs = Gcm()
 
 
-class Simulation(object):
+class Simulation():
     def __init__(self, parent, num=None):
         if num is not None and isinstance(num, int) and \
            num not in Gcs.get_all_managers():
             self.num = num
         else:
             self.num = Gcs.get_next_num()
         Gcs.set_active(self)
@@ -98,14 +97,16 @@
                     rtn = self._process_response(resp)
                     if resp.get('id', -1) == cid:
                         return rtn
             return True
         except:
             traceback.print_exc(file=sys.stdout)
 
+        return False
+
     def is_valid(self):
         return self.status['valid']
 
     def is_running(self):
         return self.status['running']
 
     def wait_until_simulation_paused(self, timeout=None):
@@ -138,15 +139,15 @@
         self.stop()
         self.qresp = mp.Queue()
         self.qcmd = mp.Queue()
         self.sim_process = mp.Process(target=sim_process,
                                       args=(self.qresp, self.qcmd))
         self.sim_process.start()
         self._interfaces = self._send_command('get_interfaces')
-        if self._set_interfaces:
+        if self._interfaces:
             self._set_interfaces(self._interfaces)
 
     def _set_interfaces(self, interfaces):
         for item in interfaces:
             if hasattr(self, item):
                 continue
 
@@ -155,18 +156,17 @@
 
             formatted_args = interfaces[item]['args']
             formatted_args = formatted_args.lstrip('(').rstrip(')')
             formatted_args2 = []
             for arg in formatted_args.split(','):
                 if '=' in arg:
                     # remove the default value
-                    arg = arg[:arg.find('=')]
-                    arg = "{0}={0}".format(arg)
+                    arg = arg[:arg.find('=')].strip()
+                    arg = f"{arg}={arg}"
                 formatted_args2.append(arg)
-
             fndef = 'lambda %s: wrapper("%s", %s)' % (
                 formatted_args, item, ','.join(formatted_args2))
             fake_fn = eval(fndef, {'wrapper': wrapper, 'item': item})
             fake_fn.__doc__ = interfaces[item]['doc']
             setattr(self, item, fake_fn)
 
     def load(self, filename=None, block=True):
@@ -230,18 +230,18 @@
             return objs
         else:
             raise ValueError()
 
     def global_object_name(self, obj):
         """generate the global name for simulation object (num.name)"""
         if obj in self.objects:
-            return "%d." % self.num + obj
+            return f"{self.num}.{obj}"
         return None
 
-    def monitor(self, objects, grid=None, index=-1):
+    def monitor(self, objects, grid=None, index=-1, style='Text', **kwargs):
         """
         show the register in a propgrid window
 
         grid: If the grid is None, the objects will be added to the active propgrid
         window. If the active propgrid window is also None, it will create one.
 
         index: the index of the object in the propgrid window. -1 to append.
@@ -258,24 +258,26 @@
         for name in self._object_list(objects):
             obj = self.objects.get(name, None)
             # ignore the invalid object
             if obj is None:
                 print("invalid object: ", name)
                 continue
             if obj['kind'] == 'sc_module':
-                prop = grid.InsertSeparator(
-                    self.global_object_name(obj['name']), obj['basename'],
-                    index)
+                prop = PropSim('Separator', label=obj['basename'], **kwargs)
+                prop.Name(self.global_object_name(obj['name']))
+                # call insert after set the name as "Insert" will trigger
+                # the monitor_signal command
+                prop = grid.Insert(prop, index)
             else:
-                prop = grid.InsertProperty(
-                    self.global_object_name(obj['name']), obj['basename'],
-                    obj['value'], index)
+                prop = PropSim(style, label=obj['basename'], **kwargs)
+                prop.Name(self.global_object_name(obj['name'])).Value(obj['value'])
                 prop.SetGripperColor(self.frame.GetColor())
+                prop = grid.Insert(prop, index)
                 if not obj['writable']:
-                    prop.SetControlStyle('none')
+                    prop.Editing(False)
                 prop.SetShowCheck(obj['readable'])
                 # set value invalid since obj['value'] may have garbage value
                 # (not read the actual value from simulation yet.);
                 # will set it to true once the value is updated.
                 prop.SetValueValid(False)
             props.append(prop)
             if index != -1:
@@ -309,14 +311,16 @@
                     self.read(objects=[], block=False)
                     self.read_buf([], block=False)
                 self.status.update(value)
             return value
         except:
             traceback.print_exc(file=sys.stdout)
 
+        return None
+
     def process_response(self):
         if not self.qresp:
             return None
         try:
             # process the response
             resp = self.qresp.get_nowait()
             if resp:
@@ -336,20 +340,18 @@
 class ModuleTree(FastLoadTreeCtrl):
     """the tree control to show the hierarchy of the objects in the simulation"""
     def __init__(self, parent, style=wx.TR_DEFAULT_STYLE):
         style = style | wx.TR_HAS_VARIABLE_ROW_HEIGHT | wx.TR_HIDE_ROOT |\
                 wx.TR_MULTIPLE | wx.TR_LINES_AT_ROOT
         FastLoadTreeCtrl.__init__(self, parent, self.get_children, style=style)
         imglist = wx.ImageList(16, 16, True, 10)
-        for xpm in [
-                module_xpm, switch_xpm, in_xpm, out_xpm, inout_xpm,
-                module_grey_xpm, switch_grey_xpm, in_grey_xpm, out_grey_xpm,
-                inout_grey_xpm
+        for svg in [
+                module_svg, signal_svg, input_svg, output_svg, inout_svg,
         ]:
-            imglist.Add(wx.Bitmap(to_byte(xpm)))
+            imglist.Add(svg_to_bitmap(svg, win=self))
         self.AssignImageList(imglist)
         self.objects = None
 
     def get_children(self, item):
         """ callback function to return the children of item """
         if item == self.GetRootItem():
             parent = ""
@@ -385,22 +387,32 @@
                 children.append(child)
         return children
 
     def OnCompareItems(self, item1, item2):
         """compare the two items for sorting"""
         def SortByName(obj1, obj2):
             """compare the two items based on its type and name"""
-            type1 = obj1['nkind'] in [SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY]
-            type2 = obj2['nkind'] in [SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY]
-            if type1 == type2:
-                if obj1['name'] > obj2['name']:
-                    return 1
-            elif type1 < type2:
-                return 1
-            return -1
+            type1 = obj1['nkind']# in [SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY]
+            type2 = obj2['nkind']# in [SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY]
+            order = [SC_OBJ_MODULE, SC_OBJ_XSC_ARRAY, SC_OBJ_CLOCK, SC_OBJ_INPUT,
+                     SC_OBJ_INOUT, SC_OBJ_OUTPUT, SC_OBJ_SIGNAL, SC_OBJ_XSC_PROP,
+                     SC_OBJ_XSC_ARRAY_ITEM, SC_OBJ_UNKNOWN]
+            type1_order = len(order)
+            type2_order = len(order)
+            if type1 in order:
+                type1_order = order.index(type1)
+            if type2 in order:
+                type2_order = order.index(type2)
+
+            if type1_order == type2_order and obj1['name'] == obj2['name']:
+                return 0
+            if type1_order == type2_order:
+                return 1 if obj1['name'] > obj2['name'] else -1
+
+            return 1 if type1_order > type2_order else -1
 
         data1 = self.GetExtendObj(item1)
         data2 = self.GetExtendObj(item2)
         rtn = -2
         if data1 and data2:
             return SortByName(data1, data2)
         return rtn
@@ -513,20 +525,25 @@
                                         initial=256)
             szSize.Add(self.spinSize, 1, wx.EXPAND | wx.ALL, 5)
             szAll.Add(szSize, 0, wx.ALL | wx.EXPAND, 5)
 
         self.m_staticline1 = wx.StaticLine(self, style=wx.LI_HORIZONTAL)
         szAll.Add(self.m_staticline1, 0, wx.EXPAND | wx.ALL, 5)
 
-        szConfirm = wx.BoxSizer(wx.HORIZONTAL)
-        self.btnOK = wx.Button(self, wx.ID_OK, u"OK")
-        szConfirm.Add(self.btnOK, 0, wx.ALL, 5)
-        self.btnCancel = wx.Button(self, wx.ID_CANCEL, u"Cancel")
-        szConfirm.Add(self.btnCancel, 0, wx.ALL, 5)
-        szAll.Add(szConfirm, 0, wx.ALIGN_RIGHT, 5)
+        btnsizer = wx.StdDialogButtonSizer()
+
+        self.btnOK = wx.Button(self, wx.ID_OK)
+        self.btnOK.SetDefault()
+        btnsizer.AddButton(self.btnOK)
+
+        self.btnCancel = wx.Button(self, wx.ID_CANCEL)
+        btnsizer.AddButton(self.btnCancel)
+        btnsizer.Realize()
+
+        szAll.Add(btnsizer, 0, wx.ALIGN_RIGHT, 5)
 
         self.SetSizer(szAll)
         self.Layout()
         szAll.Fit(self)
 
         self.tcValid.Enable(self.cbTrigger.GetValue())
         # Connect Events
@@ -586,45 +603,114 @@
             self.trace['valid'] = self.tcValid.GetValue()
         self.trace['trigger'] = self.rbTrigger.GetSelection()
         event.Skip()
 
     def GetTrace(self):
         return self.trace
 
+class DumpManageDlg(wx.Dialog):
+    ID_MP_DUMP_STOP = wx.NewId()
+    def __init__(self, sim, parent, id=-1, title='Manage dump files',
+                 size=wx.DefaultSize, pos=wx.DefaultPosition,
+                 style=wx.DEFAULT_DIALOG_STYLE|wx.RESIZE_BORDER):
+        wx.Dialog.__init__(self)
+        self.SetExtraStyle(wx.DIALOG_EX_CONTEXTHELP)
+        self.Create(parent, id, title, pos, size, style)
+
+        self.propgrid = pg.PropGrid(self)
+        g = self.propgrid
+        g.Draggable(False)
+        g.Configurable(False)
+        self.sim = sim
+
+        dumps = sim.get_trace_files()
+        for f, opt in dumps.items():
+            g.Insert(pg.PropSeparator(f)).Expand(False)
+            for name, value in self.GetDumpDescription(opt):
+                g.Insert(pg.PropText(name)).Value(value).Editing(False).Indent(1)
+
+        sizer = wx.BoxSizer(wx.VERTICAL)
+
+        sizer.Add(g, 1, wx.EXPAND|wx.ALL, 1)
+
+        # ok/cancel button
+        btnsizer = wx.StdDialogButtonSizer()
+        btnsizer.AddStretchSpacer(1)
+
+        btn = wx.Button(self, wx.ID_OK)
+        btn.SetDefault()
+        btnsizer.AddButton(btn)
+
+        btn = wx.Button(self, wx.ID_CANCEL)
+        btnsizer.AddButton(btn)
+        btnsizer.Realize()
+
+        sizer.Add(btnsizer, 0, wx.ALL|wx.EXPAND, 5)
+
+        self.SetSizer(sizer)
+
+        g.Bind(pg.EVT_PROP_RIGHT_CLICK, self.OnPropEventsHandler)
+
+    def OnPropEventsHandler(self, event):
+        prop = event.GetProp()
+        if isinstance(prop, pg.PropSeparator):
+            menu = wx.Menu()
+            menu.Append(self.ID_MP_DUMP_STOP, 'Stop dumpping file')
+            cmd = PopupMenu(self, menu)
+
+            if cmd == self.ID_MP_DUMP_STOP:
+                filename = prop.GetLabel()
+                msg = f"Do you want to stop dumping {filename}?"
+                dlg = wx.MessageDialog(self, msg, 'bsmedit', wx.YES_NO)
+                result = dlg.ShowModal() == wx.ID_YES
+                dlg.Destroy()
+                if result:
+                    if self.sim.close_trace_file(filename):
+                        prop.SetEnable(False)
+
+    def GetDumpDescription(self, dump):
+        formats = {0: 'VCD', 1:'BSM'}
+        edge = {0:"pos edge", 1: "neg edge", 2:"both edge"}
+        trigger = dump[3]
+        if trigger is None:
+            trigger = ''
+        info = [['signal', dump[1]],
+                ['trigger', f'{trigger} @ {edge.get(dump[4], "unknown edge")}'],
+                ['format', formats.get(dump[2], 'unknown')]
+                ]
+        return info
 
 class SimPanel(wx.Panel):
     ID_SIM_STEP = wx.NewId()
     ID_SIM_RUN = wx.NewId()
     ID_SIM_PAUSE = wx.NewId()
     ID_SIM_SET = wx.NewId()
     ID_MP_DUMP = wx.NewId()
     ID_MP_TRACE_BUF = wx.NewId()
     ID_MP_ADD_TO_NEW_VIEWER = wx.NewId()
     ID_MP_ADD_TO_VIEWER_START = wx.NewId()
+    ID_MP_DUMP_MANAGE = wx.NewId()
 
     def __init__(self, parent, num=None, filename=None, silent=False):
         wx.Panel.__init__(self, parent)
 
         self.is_destroying = False
         self._color = wx.Colour(178, 34, 34)
         self.toolbarart = AuiToolBarPopupArt(self)
-        self.tb = aui.AuiToolBar(self,
-                                 -1,
-                                 agwStyle=aui.AUI_TB_OVERFLOW
-                                 | aui.AUI_TB_PLAIN_BACKGROUND)
+        self.tb = aui.AuiToolBar(self, -1, agwStyle=aui.AUI_TB_OVERFLOW)
         self.tb.SetToolBitmapSize(wx.Size(16, 16))
         xpm2bmp = wx.Bitmap
-        self.tb.AddTool(self.ID_SIM_STEP, "Step", svg_to_bitmap(step_svg),
-                        svg_to_bitmap(step_grey_svg), wx.ITEM_NORMAL,
+        self.tb.AddTool(self.ID_SIM_STEP, "Step", svg_to_bitmap(step_svg, win=self),
+                        svg_to_bitmap(step_grey_svg, win=self), wx.ITEM_NORMAL,
                         "Step the simulation")
-        self.tb.AddTool(self.ID_SIM_RUN, "Run", svg_to_bitmap(run_svg),
-                        svg_to_bitmap(run_grey_svg), wx.ITEM_NORMAL,
+        self.tb.AddTool(self.ID_SIM_RUN, "Run", svg_to_bitmap(run_svg, win=self),
+                        svg_to_bitmap(run_grey_svg, win=self), wx.ITEM_NORMAL,
                         "Run the simulation")
-        self.tb.AddTool(self.ID_SIM_PAUSE, "Pause", svg_to_bitmap(pause_svg),
-                        svg_to_bitmap(pause_grey_svg), wx.ITEM_NORMAL,
+        self.tb.AddTool(self.ID_SIM_PAUSE, "Pause", svg_to_bitmap(pause_svg, win=self),
+                        svg_to_bitmap(pause_grey_svg, win=self), wx.ITEM_NORMAL,
                         "Pause the simulation")
 
         self.tb.AddSeparator()
 
         self.tcStep = wx.SpinCtrlDouble(self.tb,
                                         value='1000',
                                         size=(150, -1),
@@ -655,15 +741,15 @@
         self.cmbUnitTotal = wx.Choice(self.tb,
                                       wx.ID_ANY,
                                       size=(50, -1),
                                       choices=units)
         self.cmbUnitTotal.SetSelection(2)
         self.tb.AddControl(self.cmbUnitTotal)
         self.tb.AddStretchSpacer()
-        self.tb.AddSimpleTool(self.ID_SIM_SET, "Setting", xpm2bmp(to_byte(setting_xpm)),
+        self.tb.AddSimpleTool(self.ID_SIM_SET, "Setting", svg_to_bitmap(setting_svg, win=self),
                               "Configure the simulation")
 
         self.tb.SetToolDropDown(self.ID_SIM_SET, True)
         self.tb.SetArtProvider(self.toolbarart)
         self.tb.Realize()
         self.tree = ModuleTree(self)
         self.box = wx.BoxSizer(wx.VERTICAL)
@@ -702,14 +788,18 @@
             self.sim.process_response()
         except:
             traceback.print_exc(file=sys.stdout)
 
     def OnMenuDropDown(self, event):
         if event.IsDropDownClicked():
             menu = wx.Menu()
+            item = menu.Append(self.ID_MP_DUMP_MANAGE, "&Manage dump files")
+            if not self.sim.get_trace_files():
+                item.Enable(False)
+            menu.AppendSeparator()
             menu.Append(wx.ID_RESET, "&Reset")
             menu.AppendSeparator()
             menu.Append(wx.ID_EXIT, "&Exit")
 
             # line up our menu with the button
             tb = event.GetEventObject()
             tb.SetToolSticky(event.GetId(), True)
@@ -729,15 +819,15 @@
         dp.disconnect(receiver=self._process_response,
                       signal='sim.response',
                       sender=self.sim)
         self.timer.Stop()
         self.is_destroying = True
         self.sim.release()
         self.sim = None
-        super(SimPanel, self).Destroy()
+        super().Destroy()
 
     def SetColor(self, clr):
         self._color = clr
 
     def GetColor(self):
         return self._color
 
@@ -748,15 +838,15 @@
 
         step = self.tcStep.GetValue()
         unitStep = self.cmbUnitStep.GetString(self.cmbUnitStep.GetSelection())
         step = "%f%s" % (step, unitStep)
         total = self.tcTotal.GetValue()
         unitTotal = self.cmbUnitTotal.GetString(
             self.cmbUnitTotal.GetSelection())
-        total = "%f%s" % (total, unitTotal)
+        total = f"%f%s" % (total, unitTotal)
         self.sim.set_parameter(step=step, total=total, block=block)
 
     def OnTreeSelChanged(self, event):
         item = event.GetItem()
         if not item.IsOk():
             return
         # pre-read the prop value
@@ -769,17 +859,17 @@
             wx.CallAfter(self.sim.read, objects, block=True)
 
     def OnTreeItemMenu(self, event):
         item = event.GetItem()
         if not item.IsOk():
             return
         menu = wx.Menu()
-        menu.Append(self.ID_MP_DUMP, "&Dump file")
+        menu.Append(self.ID_MP_DUMP, "&Dump to file")
         menu.AppendSeparator()
-        menu.Append(self.ID_MP_TRACE_BUF, "&Trace buffer")
+        menu.Append(self.ID_MP_TRACE_BUF, "&Trace to buffer")
         menu.AppendSeparator()
         submenu = wx.Menu()
         submenu.Append(self.ID_MP_ADD_TO_NEW_VIEWER, "&Add to new propgrid")
         submenu.AppendSeparator()
         nid = wx.ID_HIGHEST
         grids = []
         for mag in SimPropGrid.GCM.get_all_managers():
@@ -900,19 +990,18 @@
         eid = event.GetId()
         if eid in [self.ID_SIM_STEP, self.ID_SIM_RUN]:
             event.Enable(self.sim and not self.sim.is_running())
         elif eid == self.ID_SIM_PAUSE:
             event.Enable(self.sim and self.sim.is_running())
 
     def _exit_sim(self):
-        msg = 'Do you want to kill %s?' % (self.GetLabel())
+        msg = f'Do you want to kill {self.GetLabel()}?'
         # use top level frame as parent, otherwise it may crash when
         # it is called in Destroy()
-        dlg = wx.MessageDialog(self.GetTopLevelParent(), msg, 'bsmedit',
-                               wx.YES_NO)
+        dlg = wx.MessageDialog(self.GetTopLevelParent(), msg, 'bsmedit', wx.YES_NO)
         result = dlg.ShowModal() == wx.ID_YES
         dlg.Destroy()
         if result:
             self.sim.stop()
             wx.CallAfter(dp.send, signal='frame.delete_panel', panel=self)
 
     def OnProcessCommand(self, event):
@@ -928,14 +1017,18 @@
             self.SetParameter(False)
             self.sim.step()
         elif eid == self.ID_SIM_RUN:
             self.SetParameter(False)
             self.sim.run()
         elif eid == self.ID_SIM_PAUSE:
             self.sim.pause()
+        elif eid == self.ID_MP_DUMP_MANAGE:
+            dlg = DumpManageDlg(self.sim, self, size=(600, 480))
+            # this does not return until the dialog is closed.
+            val = dlg.ShowModal()
 
     def _process_response(self, resp):
         if self.is_destroying:
             return
         try:
             command = resp.get('cmd', '')
             value = resp.get('value', False)
@@ -981,15 +1074,15 @@
                 bp = value  #[name, condition, hitcount, hitsofar]
                 gname = self.sim.global_object_name
                 for grid in SimPropGrid.GCM.get_all_managers():
                     if grid.TriggerBreakPoint(gname(bp[0]), bp[1], bp[2]):
                         dp.send(signal='frame.show_panel', panel=grid)
                         break
                 else:
-                    txt = "Breakpoint triggered: %s\n" % (json.dumps(bp))
+                    txt = f"Breakpoint triggered: {json.dumps(bp)}\n"
                     dp.send(signal='shell.write_out', text=txt)
             elif command == 'write_out':
                 dp.send(signal='shell.write_out', text=value)
 
             if command in ['load', 'step'] and value:
                 self.sim.time_stamp(insecond=False, block=False)
                 self.sim.read(objects=[], block=False)
@@ -998,97 +1091,139 @@
             traceback.print_exc(file=sys.stdout)
 
 
 wxEVT_PROP_CLICK_CHECK = wx.NewEventType()
 EVT_PROP_CLICK_CHECK = wx.PyEventBinder(wxEVT_PROP_CLICK_CHECK, 1)
 
 
-class SimProperty(pg.Property):
-    def __init__(self, grid, name, label, value):
-        pg.Property.__init__(self, grid, name, label, value)
-        self.gripper_clr = wx.RED
-        self.show_check = True
-        self.checked = False
-        self.condition = ("", "")
-        self.triggered = False
+class PropSim(pg.PropBase):
+    def __init__(self, style='Text', *args, **kwargs):
+        self.prop = None
+        self.SetControlStyle(style, *args, **kwargs)
+
+    def all_subclasses(self):
+        def _sub_classes(cls):
+            return set(cls.__subclasses__()).union(
+                    [s for c in cls.__subclasses__() for s in _sub_classes(c)])
+        sub =  _sub_classes(pg.PropBase)
+        return {s.__name__: s for s in sub if sub != PropSim}
+
+    def __getattr__(self, name):
+        return getattr(self.prop, name)
+
+    def SetControlStyle(self, style, *args, **kwargs):
+        sub = self.all_subclasses()
+        cls = sub.get(style, None)
+        if cls is None:
+            cls = sub.get(f'Prop{style}', None)
+        if cls is None:
+            cls = sub.get(f'Prop{style.title()}', None)
+        if cls is None:
+            return False
+
+        if isinstance(self.prop, cls):
+            return True
+        prop = cls(*args, **kwargs)
+        if self.prop:
+            prop.copy(self.prop)
+        self.prop = prop
+        return True
 
     def duplicate(self):
-        p = super(SimProperty, self).duplicate()
-        p.gripper_clr = self.gripper_clr
-        p.show_check = self.show_check
-        p.checked = self.checked
+        p = PropSim()
+        if self.prop:
+            p.prop = self.prop.duplicate()
         return p
 
+def PropGenericUdpate():
+    pg.PropGeneric.gripper_clr = wx.RED
+    pg.PropGeneric.show_check = True
+    pg.PropGeneric.checked = False
+    pg.PropGeneric.condition = ("", "")
+    pg.PropGeneric.triggered = False
     def SetGripperColor(self, clr=None):
         self.gripper_clr = clr
+    pg.PropGeneric.SetGripperColor = SetGripperColor
 
     def GetGripperColor(self):
         return self.gripper_clr
+    pg.PropGeneric.GetGripperColor = GetGripperColor
 
     def SetShowCheck(self, show=True, silent=True):
         """show/hide radio button"""
         if self.show_check == show:
             return
         self.show_check = show
         if not silent:
             self.Refresh()
+    pg.PropGeneric.SetShowCheck = SetShowCheck
 
     def IsShowCheck(self):
         """return whether the icon is shown"""
         return self.show_check
+    pg.PropGeneric.IsShowCheck = IsShowCheck
 
     def SetChecked(self, check=True, silent=False):
         """check/uncheck the radio button"""
         if check != self.IsChecked():
             self.checked = check
             if not self.SendPropEvent(wxEVT_PROP_CLICK_CHECK):
                 self.checked = not check
             if not silent:
                 self.Refresh()
 
+    pg.PropGeneric.SetChecked = SetChecked
+
     def IsChecked(self):
         """return true if the radio button is checked"""
         return self.checked
 
+    pg.PropGeneric.IsChecked = IsChecked
+
     def OnMouseUp(self, pt):
         ht = self.HitTest(pt)
         if self.IsEnabled():
             # click on the check icon? change the state
             if self.IsShowCheck() and ht == 'check':
                 checked = self.IsChecked()
                 self.SetChecked(not checked)
         return ht
+    pg.PropGeneric.OnMouseUp = OnMouseUp
 
     def SetBpConditon(self, cond, hitcount):
         self.condition = (cond, hitcount)
+    pg.PropGeneric.SetBpConditon = SetBpConditon
 
     def GetBpCondition(self):
         return self.condition
+    pg.PropGeneric.GetBpCondition = GetBpCondition
 
     def SetTriggered(self, triggered):
         self.triggered = triggered
+    pg.PropGeneric.SetTriggered = SetTriggered
 
     def IsTriggered(self):
         return self.triggered
+    pg.PropGeneric.IsTriggered = IsTriggered
 
 class SimPropArt(pg.PropArtNative):
-    def __init__(self):
-        super(SimPropArt, self).__init__()
+    def __init__(self, win=None):
+        super().__init__()
         self.gripper_width = 6
         if wx.Platform == '__WXMSW__':
             self.img_expand = wx.ImageList(12, 12, True, 2)
             self.img_expand.Add(wx.Bitmap(to_byte(pg.tree_xpm)))
             self.expansion_width = 12
         self.check_width = 16
         sx, sy = 16, 16
         self.img_check = wx.ImageList(sx, sy, True, 4)
-        self.img_check.Add(svg_to_bitmap(radio_unchecked_svg, width=sx, height=sy))
-        self.img_check.Add(svg_to_bitmap(radio_disabled_svg, width=sx, height=sy))
-        self.img_check.Add(svg_to_bitmap(radio_checked_svg, width=sx, height=sy))
-        self.img_check.Add(svg_to_bitmap(radio_activated_svg, width=sx, height=sy))
+        self.img_check.Add(svg_to_bitmap(radio_unchecked_svg, width=sx, height=sy, win=win))
+        self.img_check.Add(svg_to_bitmap(radio_disabled_svg, width=sx, height=sy, win=win))
+        self.img_check.Add(svg_to_bitmap(radio_checked_svg, width=sx, height=sy, win=win))
+        self.img_check.Add(svg_to_bitmap(radio_activated_svg, width=sx, height=sy, win=win))
         #self.img_check.Add(wx.Bitmap(to_byte(pg.radio_xpm)))
 
     def PrepareDrawRect(self, p):
         """calculate the rect for each section"""
         mx = self.gap_x
         irc = p.GetRect()
         irc.SetLeft(irc.GetLeft() + self.margin['left'])
@@ -1204,18 +1339,18 @@
                 y = rc.y + (rc.height - h) / 2 + 1
                 idx = 0
                 if not p.IsExpanded():
                     idx = 1
                 self.img_expand.Draw(idx, dc, x, y,
                                      wx.IMAGELIST_DRAW_TRANSPARENT)
             else:
-                super(SimPropArt, self).DrawExpansion(dc, p)
+                super().DrawExpansion(dc, p)
 
     def DrawItem(self, dc, p):
-        super(SimPropArt, self).DrawItem(dc, p)
+        super().DrawItem(dc, p)
         self.DrawGripper(dc, p)
         self.DrawCheck(dc, p)
 
 
 class SimPropGrid(pg.PropGrid):
     GCM = Gcm()
     ID_PROP_BREAKPOINT = wx.NewId()
@@ -1225,38 +1360,37 @@
         pg.PropGrid.__init__(self, parent)
 
         # if num is not defined or is occupied, generate a new one
         if num is None or num in SimPropGrid.GCM.get_nums():
             num = SimPropGrid.GCM.get_next_num()
         self.num = num
         SimPropGrid.GCM.set_active(self)
-        self.SetArtProvider(SimPropArt())
-        self._prop_cls = SimProperty
+        self.SetArtProvider(SimPropArt(self))
         self.Bind(EVT_PROP_CLICK_CHECK, self.OnPropEventsHandler)
 
         dp.connect(self.OnSimLoad, 'sim.loaded')
         dp.connect(self.OnSimUnload, 'sim.unloaded')
         dp.connect(self.OnSimUpdate, 'sim.update')
 
     def Destroy(self):
         dp.disconnect(self.OnSimLoad, 'sim.loaded')
         dp.disconnect(self.OnSimUnload, 'sim.unloaded')
         dp.disconnect(self.OnSimUpdate, 'sim.update')
-        self.DeleteAllProperties()
+        self.DeleteAll()
         SimPropGrid.GCM.destroy_mgr(self)
-        super(SimPropGrid, self).Destroy()
+        super().Destroy()
 
     def OnSimUpdate(self, objs):
         for name, v in six.iteritems(objs):
-            p = self.GetProperty(name)
+            p = self.Get(name)
             if isinstance(p, list):
                 for prop in p:
                     prop.SetValue(v)
                     prop.SetValueValid(True)
-            elif isinstance(p, pg.Property):
+            elif isinstance(p, pg.PropBase):
                 p.SetValue(v)
                 p.SetValueValid(True)
 
     def OnSimLoad(self, num):
         """try reconnecting registers when the simulation is loaded."""
         s = str(num) + '.'
         sl = len(s)
@@ -1270,24 +1404,24 @@
             resp = dp.send('sim.command',
                            num=num,
                            command='monitor_signal',
                            objects=objs)
             if not resp:
                 return
             status = resp[0][1]
-            if status == False:
+            if status is False:
                 return
             for obj in objs:
                 # enable props that is monitored successfully
                 if isinstance(status, dict) and not status.get(obj, False):
                     continue
-                p = self.GetProperty(s + obj)
+                p = self.Get(s + obj)
                 if not p:
                     continue
-                if isinstance(p, pg.Property):
+                if isinstance(p, pg.PropBase):
                     p = [p]
                 for prop in p:
                     prop.SetReadonly(False)
                     prop.Enable(True)
 
     def OnSimUnload(self, num):
         # disable all props from the simulation with id 'num'
@@ -1296,30 +1430,30 @@
             name = p.GetName()
             if not name.startswith(s):
                 continue
             p.SetReadonly(True)
             p.Enable(False)
 
     def GetContextMenu(self, prop):
-        menu = super(SimPropGrid, self).GetContextMenu(prop)
+        menu = super().GetContextMenu(prop)
         if not menu:
             menu = wx.Menu()
         else:
             menu.AppendSeparator()
         if prop:
             menu.Append(self.ID_PROP_BREAKPOINT, "Breakpoint Condition")
             menu.Enable(self.ID_PROP_BREAKPOINT, prop.IsChecked())
         menu.Append(self.ID_PROP_BREAKPOINT_CLEAR, "Clear all Breakpoints")
         return menu
 
     def OnPropEventsHandler(self, evt):
-        if not super(SimPropGrid, self).OnPropEventsHandler(evt):
+        if not super().OnPropEventsHandler(evt):
             return False
 
-        prop = evt.GetProperty()
+        prop = evt.GetProp()
         eid = evt.GetEventType()
         if eid == wxEVT_PROP_CLICK_CHECK:
             # turn on/off breakpoint
             if prop.IsChecked():
                 dp.send('prop.bp_add', prop=prop)
             else:
                 dp.send('prop.bp_del', prop=prop)
@@ -1344,15 +1478,15 @@
                     prop.SetChecked(True)
                 else:
                     prop.SetBpConditon(*dlg.GetCondition())
 
         elif eid == self.ID_PROP_BREAKPOINT_CLEAR:
             self.ClearBreakPoints()
         else:
-            super(SimPropGrid, self).OnProcessCommand(eid, prop)
+            super().OnProcessCommand(eid, prop)
 
     def ClearBreakPoints(self):
         """clear all the breakpoints"""
         for prop in self._props:
             if prop and prop.IsChecked():
                 prop.SetChecked(False)
     @classmethod
@@ -1371,14 +1505,23 @@
                 if (cond, hitcount) == prop.GetBpCondition():
                     prop.SetTriggered(True)
                     self.EnsureVisible(prop)
                     self.SetSelection(prop)
                     return True
         return False
 
+    def Index(self, prop):
+        """return the index of prop, or -1 if not found"""
+        if isinstance(prop, pg.PropBase) and not isinstance(prop, PropSim):
+            for i, p in enumerate(self._props):
+                if prop == p.prop:
+                    return i
+            return -1
+
+        return super().Index(prop)
 
 class BreakpointSettingsDlg(wx.Dialog):
     def __init__(self, parent, condition='', hitcount=''):
         wx.Dialog.__init__(self,
                            parent,
                            title="Breakpoint Condition",
                            size=wx.Size(431, 289),
@@ -1418,23 +1561,25 @@
         szCnd.Add(szCond, 1, wx.EXPAND, 5)
 
         szAll.Add(szCnd, 1, wx.EXPAND, 5)
 
         self.stLine = wx.StaticLine(self, style=wx.LI_HORIZONTAL)
         szAll.Add(self.stLine, 0, wx.EXPAND | wx.ALL, 5)
 
-        szConfirm = wx.BoxSizer(wx.HORIZONTAL)
+        btnsizer = wx.StdDialogButtonSizer()
 
-        self.btnOK = wx.Button(self, wx.ID_OK, u"OK")
-        szConfirm.Add(self.btnOK, 0, wx.ALL, 5)
+        self.btnOK = wx.Button(self, wx.ID_OK)
+        self.btnOK.SetDefault()
+        btnsizer.AddButton(self.btnOK)
 
-        self.btnCancel = wx.Button(self, wx.ID_CANCEL, u"Cancel")
-        szConfirm.Add(self.btnCancel, 0, wx.ALL, 5)
+        self.btnCancel = wx.Button(self, wx.ID_CANCEL)
+        btnsizer.AddButton(self.btnCancel)
+        btnsizer.Realize()
 
-        szAll.Add(szConfirm, 0, wx.ALIGN_RIGHT, 5)
+        szAll.Add(btnsizer, 0, wx.ALIGN_RIGHT, 5)
 
         self.SetSizer(szAll)
         self.Layout()
 
         # initialize the controls
         self.condition = condition
         self.hitcount = hitcount
@@ -1481,21 +1626,22 @@
             self.hitcount = ""
         event.Skip()
 
     def GetCondition(self):
         return (self.condition, self.hitcount)
 
 
-class sim(object):
+class sim:
     frame = None
     ID_SIM_NEW = wx.NOT_FOUND
     ID_PROP_NEW = wx.NOT_FOUND
 
     @classmethod
     def initialize(cls, frame):
+        PropGenericUdpate()
         cls.frame = frame
 
         resp = dp.send(signal='frame.add_menu',
                        path='File:New:Simulation',
                        rxsignal='bsm.simulation')
         if resp:
             cls.ID_SIM_NEW = resp[0][1]
@@ -1505,15 +1651,15 @@
         if resp:
             cls.ID_PROP_NEW = resp[0][1]
 
         dp.connect(cls._process_command, signal='bsm.simulation')
         dp.connect(cls._sim_command, signal='sim.command')
         dp.connect(receiver=cls._frame_set_active,
                    signal='frame.activate_panel')
-        dp.connect(receiver=cls._frame_uninitialize, signal='frame.exit')
+        dp.connect(receiver=cls._frame_uninitialize, signal='frame.exiting')
         dp.connect(receiver=cls.initialized, signal='frame.initialized')
         dp.connect(receiver=cls._prop_insert, signal='prop.insert')
         dp.connect(receiver=cls._prop_delete, signal='prop.delete')
         dp.connect(receiver=cls._prop_drop, signal='prop.drop')
         dp.connect(receiver=cls._prop_bp_add, signal='prop.bp_add')
         dp.connect(receiver=cls._prop_bp_del, signal='prop.bp_del')
         dp.connect(receiver=cls._prop_changed, signal='prop.changed')
@@ -1564,14 +1710,16 @@
             cnd = prop.GetBpCondition()
             if cnd is None:
                 cnd = ("", "")
             mgr.del_breakpoint(name, cnd[0], cnd[1])
 
     @classmethod
     def _prop_insert(cls, prop):
+        if not isinstance(prop, PropSim):
+            return
         mgr, name = cls._find_object(prop.GetName())
         if mgr:
             mgr.monitor_signal(name)
 
     @classmethod
     def _prop_delete(cls, prop):
         mgr, name = cls._find_object(prop.GetName())
@@ -1611,14 +1759,17 @@
             SimPropGrid.GCM.set_active(pane)
 
     @classmethod
     def _frame_uninitialize(cls):
         for mgr in Gcs.get_all_managers():
             mgr.stop()
             dp.send('frame.delete_panel', panel=mgr.frame)
+        for mgr in SimPropGrid.GCM.get_all_managers():
+            dp.send('frame.delete_panel', panel=mgr)
+
         dp.send('frame.delete_menu', path="View:Simulations")
         dp.send('frame.delete_menu',
                 path="File:New:Simulation",
                 id=cls.ID_SIM_NEW)
         dp.send('frame.delete_menu',
                 path="File:New:PropGrid",
                 id=cls.ID_PROP_NEW)
@@ -1682,23 +1833,24 @@
 
         manager = Gcs.get_manager(num)
         if manager is None and create:
             manager = SimPanel(sim.frame, num, filename, silent)
             clr = GetColorByNum(manager.sim.num)
             clr.Set(clr.red, clr.green, clr.blue, 128)
             manager.SetColor(clr)
+            scale_factor = 1#manager.GetContentScaleFactor()
             page_bmp = MakeBitmap(clr.red, clr.green,
-                                  clr.blue)  #178,  34,  34)
-            title = "Simulation-%d" % manager.sim.num
+                                  clr.blue, scale_factor=scale_factor)
+            title = f"Simulation-{manager.sim.num}"
             dp.send(signal="frame.add_panel",
                     panel=manager,
                     title=title,
                     target="History",
                     icon=page_bmp,
-                    showhidemenu="View:Simulations:%s" % title)
+                    showhidemenu=f"View:Simulations:{title}")
             return manager.sim
         # activate the manager
         elif manager and activate:
             dp.send(signal='frame.show_panel', panel=manager)
 
         return manager
 
@@ -1708,15 +1860,15 @@
         get the propgrid handle by its number
 
         If the propgrid exists, return its handler; otherwise, it will be created.
         """
         mgr = SimPropGrid.GCM.get_manager(num)
         if not mgr and create:
             mgr = SimPropGrid(cls.frame)
-            mgr.SetLabel("Propgrid-%d" % mgr.num)
+            mgr.SetLabel(f"Propgrid-{mgr.num}")
             dp.send(signal="frame.add_panel", panel=mgr, title=mgr.GetLabel())
         elif mgr and activate:
             # activate the window
             dp.send(signal='frame.show_panel', panel=mgr)
         return mgr
 
     @classmethod
```

### Comparing `bsmedit-3.2.8/bsmedit/bsm/simprocess.py` & `bsmedit-3.2.9/bsmedit/bsm/simprocess.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/c2p.py` & `bsmedit-3.2.9/bsmedit/c2p.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/better_exchook.py` & `bsmedit-3.2.9/bsmedit/cparser/better_exchook.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/caching.py` & `bsmedit-3.2.9/bsmedit/cparser/caching.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/cparser.py` & `bsmedit-3.2.9/bsmedit/cparser/cparser.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/cparser_utils.py` & `bsmedit-3.2.9/bsmedit/cparser/cparser_utils.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/cwrapper.py` & `bsmedit-3.2.9/bsmedit/cparser/cwrapper.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/globalincludewrappers.py` & `bsmedit-3.2.9/bsmedit/cparser/globalincludewrappers.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/goto.py` & `bsmedit-3.2.9/bsmedit/cparser/goto.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/interpreter.py` & `bsmedit-3.2.9/bsmedit/cparser/interpreter.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/py_demo_unparse.py` & `bsmedit-3.2.9/bsmedit/cparser/py_demo_unparse.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/__init__.py` & `bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sorteddict.py` & `bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sorteddict.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sortedlist.py` & `bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sortedlist.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/cparser/sortedcontainers/sortedset.py` & `bsmedit-3.2.9/bsmedit/cparser/sortedcontainers/sortedset.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/frameplus.py` & `bsmedit-3.2.9/bsmedit/frameplus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import six
 import wx
-import wx.lib.agw.aui as aui
 import wx.py.dispatcher as dp
+from .aui import aui
 
 
 class AuiManagerPlus(aui.AuiManager):
     def __init__(self, managed_window=None, agwFlags=None):
         aui.AuiManager.__init__(self,
                                 managed_window=managed_window,
                                 agwFlags=agwFlags)
@@ -61,14 +61,18 @@
             for page in range(pages):
                 window = nb.GetPage(page)
                 page_pane = self.GetPane(window)
                 min_x = max(page_pane.min_size.x, min_x)
                 min_y = max(page_pane.min_size.y, min_y)
             nb_pane.MinSize(min_x, min_y)
 
+    def OnClose(self, event):
+        # AuiManager will call UnInit(), skip it and will be called by the
+        # main frame
+        event.Skip()
 
 class FramePlus(wx.Frame):
     def __init__(self,
                  parent,
                  id=wx.ID_ANY,
                  title=u'bsmedit',
                  pos=wx.DefaultPosition,
@@ -81,27 +85,28 @@
                           pos=pos,
                           size=size,
                           style=style)
         self._mgr = AuiManagerPlus()
         self._mgr.SetManagedWindow(self)
         self.menuAddon = {}
         self.paneAddon = {}
+        self.paneMenu = {}
         self._pane_num = 0
         dp.connect(self.AddMenu, 'frame.add_menu')
         dp.connect(self.DeleteMenu, 'frame.delete_menu')
         dp.connect(self.AddPanel, 'frame.add_panel')
         dp.connect(self.DeletePanel, 'frame.delete_panel')
         dp.connect(self.ShowPanel, 'frame.show_panel')
         dp.connect(self.TogglePanel, 'frame.check_menu')
         dp.connect(self.UpdateMenu, 'frame.update_menu')
         self.Bind(wx.EVT_CLOSE, self.OnClose)
 
     def OnClose(self, event):
         self._mgr.UnInit()
-        del self._mgr
+        #del self._mgr
         event.Skip()
 
     def GetMenu(self, pathlist, autocreate=False):
         """
         find the menu item.
 
         if autocreate is True, then recursive submenu creation.
@@ -264,15 +269,17 @@
                  active=True,
                  paneInfo=None,
                  target=None,
                  showhidemenu=None,
                  icon=None,
                  maximize=False,
                  direction='top',
-                 minsize=None):
+                 minsize=None,
+                 pane_menu=None,
+                 ):
         """add the panel to AUI"""
         if not panel:
             return False
         panel.Reparent(self)
         # hide the window for now to avoid flicker
         panel.Hide()
         # if the target is None, find the notebook control that has the same
@@ -316,15 +323,15 @@
                           .Row(-1).Position(99)
 
         auipaneinfo.Caption(title).DestroyOnClose(not showhidemenu).Icon(icon)\
                    .Direction(direction)
 
         if not self._mgr.GetAllPanes():
             # set the first pane to be center pane
-            auipaneinfo.CenterPane()
+            auipaneinfo.DestroyOnClose(False).CenterPane()
             active = True
 
         # auto generate the unique panel name
         name = "pane-%d" % self._pane_num
         self._pane_num += 1
         auipaneinfo.Name(name)
         if minsize:
@@ -342,25 +349,30 @@
             mid = self.AddMenu(showhidemenu,
                                rxsignal='frame.check_menu',
                                updatesignal='frame.update_menu',
                                kind='Check',
                                autocreate=True)
             if mid != wx.NOT_FOUND:
                 self.paneAddon[mid] = {'panel': panel, 'path': showhidemenu}
+        if pane_menu is not None:
+            self.paneMenu[panel] = pane_menu
         return True
 
     def DeletePanel(self, panel):
         """hide and destroy the panel"""
         # delete the show/hide menu
         for (pid, pane) in six.iteritems(self.paneAddon):
             if panel == pane['panel']:
                 self.DeleteMenu(pane['path'], pid)
                 del self.paneAddon[pid]
                 break
 
+        # delete the pane menu
+        self.paneMenu.pop(panel, None)
+
         # delete the panel from the manager
         pane = self._mgr.GetPane(panel)
         if pane is None or not pane.IsOk():
             return False
         pane.DestroyOnClose(True)
         self._mgr.ClosePane(pane)
         self._mgr.Update()
```

### Comparing `bsmedit-3.2.8/bsmedit/glsurface/_simxpm.py` & `bsmedit-3.2.9/bsmedit/glsurface/_simxpm.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/glsurface/glsurface.py` & `bsmedit-3.2.9/bsmedit/glsurface/glsurface.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/glsurface/gltest.py` & `bsmedit-3.2.9/bsmedit/glsurface/gltest.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/mainframexpm.py` & `bsmedit-3.2.9/bsmedit/mainframexpm.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/demo.py` & `bsmedit-3.2.9/bsmedit/propgrid/demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import wx
-import wx.lib.agw.aui as aui
-import wx.py as py
+from wx.lib.agw import aui
+from wx import py
+from .prop import *
 from . import propgrid as pg
 from . import formatters as fmt
 from . import enumtype
 from . import propart as pa
 from .propxpm import radio_xpm, tree_xpm
 
 
@@ -25,16 +26,16 @@
         self.text_clr_sel = self.text_clr
 
     def DrawExpansion(self, dc, p):
         if p.HasChildren():
             if self.img_expand.GetImageCount() == 2:
                 (w, h) = self.img_expand.GetSize(0)
                 rc = p.regions['expander']
-                x = rc.x + (rc.width - w) / 2
-                y = rc.y + (rc.height - h) / 2 + 1
+                x = rc.x + (rc.width - w) // 2
+                y = rc.y + (rc.height - h) // 2 + 1
                 idx = 0
                 if not p.IsExpanded():
                     idx = 1
                 self.img_expand.Draw(idx, dc, x, y,
                                      wx.IMAGELIST_DRAW_TRANSPARENT)
             else:
                 super(PropArtCustom, self).DrawExpansion(dc, p)
@@ -55,45 +56,45 @@
         else:
             clr = wx.SystemSettings.GetColour(wx.SYS_COLOUR_BTNTEXT)
         dc.SetTextForeground(clr)
         rc = p.regions['label']
         dc.SetClippingRegion(rc)
         (w, h) = dc.GetTextExtent(p.label)
 
-        dc.DrawText(p.label, rc.x, rc.y + (rc.height - h) / 2)
+        dc.DrawText(p.label, rc.x, rc.y + (rc.height - h) // 2)
         p.show_label_tips = w > rc.width
         dc.DestroyClippingRegion()
 
     def DrawSplitter(self, dc, p):
         # draw splitter
         rcs = p.regions['splitter']
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
         dc.DrawLine(rcs.right - 1, rcs.top, rcs.right - 1, rcs.bottom)
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DHILIGHT)))
         dc.DrawLine(rcs.right, rcs.top, rcs.right, rcs.bottom)
 
     def DrawBackground(self, dc, p):
         # draw background
         rc = p.GetRect()
-        rcs = p.regions['splitter']
+        rcs = p.regions.get('splitter', rc)
         bg = wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DFACE)
         brush = wx.Brush(bg)
         dc.SetBrush(brush)
         dc.DrawRectangle(rc.x, rc.y, rcs.right, rc.height)
 
     def DrawValue(self, dc, p):
         # draw value
         if p.font_value is None:
             font = self._font_value
         else:
             font = wx.Font(p.font_value)
         dc.SetFont(font)
 
         p.show_value_tips = False
-        if p.window is None:
+        if p.draws.get('value', False):
             crbg = p.bg_clr
             crtxt = wx.BLACK
             if not p.IsEnabled() or p.IsReadonly():
                 crtxt = p.text_clr_disabled
                 if not crtxt:
                     crtxt = self.text_clr_disabled
                 crbg = p.bg_clr_disabled
@@ -128,21 +129,21 @@
 
             dc.SetPen(wx.Pen(crtxt, 1, wx.PENSTYLE_TRANSPARENT))
             dc.SetTextForeground(crtxt)
 
             value = p.GetValueAsString()
             (w, h) = dc.GetTextExtent(value)
             dc.SetClippingRegion(rc)
-            dc.DrawText(value, rc.x + 5, rc.top + (rc.height - h) / 2)
+            dc.DrawText(value, rc.x + 5, rc.top + (rc.height - h) // 2)
             p.show_value_tips = rc.width < w
             dc.DestroyClippingRegion()
 
     def DrawBorder(self, dc, p):
         rc = p.GetRect()
-        rcs = p.regions['splitter']
+        rcs = p.regions.get('splitter', rc)
         # value bottom border
         crbg = p.bg_clr
         if p.IsEnabled() and not p.IsReadonly():
             crbg = p.bg_clr_disabled
             if not crbg:
                 crbg = self.bg_clr_disabled
         else:
@@ -155,18 +156,49 @@
 
         # title top & bottom border
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
         dc.DrawLine(rc.left, rc.bottom, rcs.right, rc.bottom)
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DHILIGHT)))
         dc.DrawLine(rc.left, rc.top, rcs.right, rc.top)
 
+class Prop(PropBase):
+    def __init__(self, style='Text', *args, **kwargs):
+        self.prop = None
+        self._set_style(style, *args, **kwargs)
+
+    def all_subclasses(self):
+        def _sub_classes(cls):
+            return set(cls.__subclasses__()).union(
+                    [s for c in cls.__subclasses__() for s in _sub_classes(c)])
+        sub =  _sub_classes(PropBase)
+        return {s.__name__: s for s in sub if sub != Prop}
+
+    def __getattr__(self, name):
+        return getattr(self.prop, name)
+
+    def _set_style(self, style, *args, **kwargs):
+        sub = self.all_subclasses()
+        cls = sub.get(style, None)
+        if cls is None:
+            cls = sub.get(f'Prop{style}', None)
+        if cls is None:
+            cls = sub.get(f'Prop{style.title()}', None)
+        if cls is None:
+            return False
+
+        if isinstance(self.prop, cls):
+            return True
+
+        prop = cls(*args, **kwargs)
+        self.prop = prop
+        return True
 
 class MainFrame(wx.Frame):
-    ID_ART_NATIVE = wx.NewId()
-    ID_ART_DEFAULT = wx.NewId()
+    ID_ART_NATIVE = wx.NewIdRef()
+    ID_ART_DEFAULT = wx.NewIdRef()
 
     def __init__(self):
         wx.Frame.__init__(self, None, -1, 'PropGrid Demo', size=(800, 600))
         self._mgr = aui.AuiManager()
 
         # tell AuiManager to manage this frame
         self._mgr.SetManagedWindow(self)
@@ -192,129 +224,81 @@
 
         self.Bind(wx.EVT_TOOL, self.OnProcessTool)
         self.Bind(wx.EVT_UPDATE_UI, self.OnUpdateCmdUI)
 
         self.propgrid = pg.PropGrid(self)
         g = self.propgrid
         # general
-        p = g.InsertSeparator('general', 'general')
+        g.Insert(Prop('Spin', 1, 100, 'magic')).Value(1)
+        g.Insert(PropSeparator().Label('general'))
+
+        g.Insert(PropText().Label('string').Value('hello world!').Indent(1))
+
+        g.Insert(PropText().Label('disable').Value('hello world!').Indent(1).Enable(False))
+
+        g.Insert(PropText().Label('italic').Value('hello world!').Indent(1)\
+                .ValueFont(wx.Font(wx.NORMAL_FONT).Italic()))
+
+        g.Insert(PropText().Label('bold').Value('hello world!').Indent(1)\
+             .ValueFont(wx.Font(wx.NORMAL_FONT).Bold()))
+        g.Insert(PropText().Label('not draggable').Value('hello world!').Indent(1).Draggable(False))
+
+        g.Insert(PropInt().Label('integer').Value(42).Indent(1))
+
+        g.Insert(PropHex().Label('hex').Value(42).Indent(1))
+
+        g.Insert(PropBin().Label('bin').Value( 42).Indent(1))
+
+        g.Insert(PropFloat().Label('float').Value(42.0).Indent(1))
+
+        g.Insert(PropChoice([2, 4, 8, 16, 32, 64, 128, 256]).Label('choice').Value(2).Indent(1))
 
-        p = g.InsertProperty('string', 'string', 'hello world!')
-        p.SetIndent(1)
+        g.Insert(PropDate().Label('date').Value(wx.DateTime.Today()).Indent(1))
 
-        p = g.InsertProperty('disable', 'disable', 'hello world!')
-        p.SetIndent(1)
-        p.Enable(False)
-
-        p = g.InsertProperty('italic', 'italic', 'hello world!')
-        p.SetIndent(1)
-        p.SetValueFont(wx.Font(wx.NORMAL_FONT).Italic())
-
-        p = g.InsertProperty('bold', 'bold', 'hello world!')
-        p.SetIndent(1)
-        p.SetValueFont(wx.Font(wx.NORMAL_FONT).Bold())
-
-        p = g.InsertProperty('integer', 'integer', 42)
-        p.SetIndent(1)
-        p.SetFormatter(fmt.IntFormatter())
-
-        p = g.InsertProperty('hex', 'hex', 42)
-        p.SetIndent(1)
-        p.SetFormatter(fmt.HexFormatter())
-
-        p = g.InsertProperty('bin', 'bin', 42)
-        p.SetIndent(1)
-        p.SetFormatter(fmt.BinFormatter())
-
-        p = g.InsertProperty('float', 'float', 42.0)
-        p.SetIndent(1)
-        p.SetFormatter(fmt.FloatFormatter())
-
-        p = g.InsertProperty('choice', 'choice', 2)
-        p.SetFormatter(fmt.ChoiceFormatter([2, 4, 8, 16, 32, 64, 128, 256]))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('date', 'date', wx.DateTime.Today())
-        p.SetIndent(1)
-        p.SetFormatter(fmt.DateFormatter())
-
-        p = g.InsertProperty('time', 'time', wx.DateTime.Now())
-        p.SetIndent(1)
-        p.SetFormatter(fmt.TimeFormatter())
-
-        p = g.InsertProperty('datetime', 'datetime', wx.DateTime.Now())
-        p.SetIndent(1)
-        p.SetFormatter(fmt.DateTimeFormatter())
-        p.SetControlStyle('none')
+        g.Insert(PropTime().Label('time').Value(wx.DateTime.Now()).Indent(1))
+        g.Insert(PropDateTime().Label('datetime').Value(wx.DateTime.Now()).Indent(1))
 
+        g.Insert(PropDateTime().Name('datetime').Label('datetime auto update')\
+                .Value(wx.DateTime.Now()).Indent(1).Editing(False))
         # control
-        p = g.InsertSeparator('type', 'type')
+        g.Insert(PropSeparator().Label('type'))
 
-        p = g.InsertProperty('editbox', 'editbox', 'string')
-        p.SetIndent(1)
+        g.Insert(PropEditBox().Label('editbox').Value('string').Indent(1))
 
-        p = g.InsertProperty('choice', 'choice', 1)
         choices = enumtype.EnumType(Monday=1,
                                     Tuesday=2,
                                     Wednesday=3,
                                     Thursday=4,
                                     Friday=5,
                                     Saturday=6,
-                                    Sunday=7)
-        p.SetFormatter(fmt.EnumFormatter(choices))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('dir_dialog', 'folder', '/home')
-        #p.SetControlStyle('dir_dialog')
-        p.SetFormatter(fmt.PathFormatter(False, 'folder'))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('file_dialog', 'file', '/home/temp.txt')
-        #p.SetControlStyle('file_dialog')
-        p.SetFormatter(fmt.PathFormatter(False, 'file'))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('slider', 'slider', 50)
-        p.SetControlStyle('slider')
-        p.SetFormatter(fmt.IntFormatter(1, 101))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('spin', 'spin', 50)
-        p.SetControlStyle('spin')
-        p.SetFormatter(fmt.IntFormatter(1, 100))
-        p.SetIndent(1)
-
-        p = g.InsertProperty('checkbox', 'checkbox', 0)
-        p.SetControlStyle('checkbox')
-        p.SetFormatter(fmt.BoolFormatter())
-        p.SetIndent(1)
-
-        p = g.InsertProperty('radiobox', 'radiobox', 1)
-        #p.SetFormatter(fmt.EnumFormatter(choices))
-        p.SetFormatter(
-            fmt.ChoiceFormatter({
-                1: '1',
-                0: '0',
-                'Z': 'Z',
-                'X': 'X'
-            }))
-        p.SetControlStyle('radiobox')
-        p.SetIndent(1)
-
-        p = g.InsertProperty('date', 'date', wx.DateTime.Today())
-        p.SetIndent(1)
-        p.SetFormatter(fmt.DateFormatter())
-
-        p = g.InsertProperty('time', 'time', wx.DateTime.Now())
-        p.SetIndent(1)
-        p.SetFormatter(fmt.TimeFormatter())
-
-        p = g.InsertProperty('font', 'font', wx.NORMAL_FONT)
-        p.SetIndent(1)
-        p.SetFormatter(fmt.FontFormatter())
+                                    Sunday=7)._items
+        g.Insert(PropChoice(choices).Label('choice').Value(1).Indent(1))
+
+        g.Insert(PropFolder().Label('folder').Value('./').Indent(1))
+
+        g.Insert(PropFile().Label('file').Value('./temp.txt').Indent(1))
+
+        g.Insert(PropSlider(1, 100).Label('slider').Value(50).Indent(1))
+
+        g.Insert(PropSpin(1, 100).Label('spin').Value(50).Indent(1))
+
+        g.Insert(PropCheckBox().Label('checkbox').Value(0).Indent(1))
+
+        choice = {1: '1',
+                  0: '0',
+                  'Z': 'Z',
+                  'X': 'X'
+                  }
+        g.Insert(PropRadioBox(choice).Label('radiobox').Value(1).Indent(1))
+
+        g.Insert(PropDate().Label('date').Value(wx.DateTime.Today()).Indent(1))
+
+        g.Insert(PropTime().Label('time').Value(wx.DateTime.Now()).Indent(1))
+
+        g.Insert(PropFont().Label('font').Value(wx.NORMAL_FONT).Indent(1))
 
         # color
         self.clr_map = np.array(
             [[170., 110., 40., 255.], [0., 0., 128., 255.],
              [255., 225., 25., 255.], [128., 128., 128., 255.],
              [128., 0., 0., 255.], [0., 128., 128., 255.], [0., 0., 0., 255.],
              [210., 245., 60., 255.], [250., 190., 190., 255.],
@@ -322,28 +306,23 @@
              [240., 50., 230., 255.], [230., 25., 75., 255.],
              [255., 255., 255., 255.], [230., 190., 255., 255.],
              [255., 215., 180., 255.], [60., 180., 75., 255.],
              [255., 250., 200., 255.], [245., 130., 48., 255.],
              [0., 130., 200., 255.], [70., 240., 240., 255.],
              [170., 255., 195., 255.]]) / 255
         chex = self.rgb2hex(self.clr_map[:, :-1])
-        p = self.propgrid.InsertSeparator("color", "color")
+        p = g.Insert(PropSeparator().Label("color"))
         for i, c in enumerate(chex):
-            p = self.propgrid.InsertProperty("clr-%d" % i, '%d' % i,
-                                             wx.Colour(c))
-            p.SetBgColor(c, c, c)
-            p.SetFormatter(fmt.ColorFormatter())
             t = wx.Colour(c)
             t.SetRGB(t.GetRGB() ^ 0xFFFFFF)
             t = t.GetAsString(wx.C2S_HTML_SYNTAX)
-            p.SetTextColor(t, t, t)
-            p.SetIndent(1)
+            g.Insert(PropColor().Label(f'{i}').Value(wx.Colour(c)).BgColor(c, c, c)\
+                .TextColor(t, t, t).Indent(1))
 
-        pane_grid = aui.AuiPaneInfo().Name("propgrid").Caption("PropGrid").\
-                    CenterPane()
+        pane_grid = aui.AuiPaneInfo().Name("propgrid").Caption("PropGrid").CenterPane()
         self._mgr.AddPane(self.propgrid, pane_grid)
         ns = {}
         ns['wx'] = wx
         ns['app'] = wx.GetApp()
         ns['frame'] = self
         self.shell = py.shell.Shell(self, -1, locals=ns)
 
@@ -353,55 +332,34 @@
                           .Row(-1).Bottom().Position(99)
 
         self._mgr.AddPane(self.shell, pane_shell)
         self._mgr.ShowPane(g, True)
         self._mgr.MinimizePane(pane_shell)
         self._mgr.Update()
 
-        self.Bind(pg.EVT_PROP_CHANGED, self.OnPropChanged, id=wx.ID_ANY)
-
         self.timer = wx.Timer(self)
         self.Bind(wx.EVT_TIMER, self.OnTimer, self.timer)
         self.timer.Start(100)
 
     def rgb2hex(self, clr):
         clr = np.sum(clr * 255 * [2**16, 2**8, 1], 1).astype(np.int32)
         return ["#{:06x}".format(c) for c in clr]
 
-    def OnPropChanged(self, evt):
-        p = evt.GetProperty()
-        if p.GetName().startswith('clr-'):
-            idx = int(p.GetLabel())
-            if idx >= 0 and idx < len(self.clr_map):
-                t = wx.Colour(p.GetValue())
-                self.clr_map[idx] = [
-                    t.Red() / 255.,
-                    t.Green() / 255.,
-                    t.Blue() / 255., 1.
-                ]
-                c = t.GetAsString(wx.C2S_HTML_SYNTAX)
-                p.SetBgColor(c, c, c)
-                t.SetRGB(t.GetRGB() ^ 0xFFFFFF)
-                t = t.GetAsString(wx.C2S_HTML_SYNTAX)
-                p.SetTextColor(t, t, t)
-        if 'font' in p.GetName():
-            p.SetValueFont(p.GetValue())
-
     def OnTimer(self, event):
-        p = self.propgrid.GetProperty('datetime')
+        p = self.propgrid.Get('datetime')
         if p:
             p.SetValue(wx.DateTime.Now())
 
     def OnUpdateCmdUI(self, event):
         eid = event.GetId()
         if eid == self.ID_ART_NATIVE:
             event.Check(
-                type(self.propgrid.GetArtProvider()) == pa.PropArtNative)
+                not isinstance(self.propgrid.GetArtProvider(), PropArtCustom))
         elif eid == self.ID_ART_DEFAULT:
-            event.Check(type(self.propgrid.GetArtProvider()) == PropArtCustom)
+            event.Check(isinstance(self.propgrid.GetArtProvider(), PropArtCustom))
         else:
             event.Skip()
 
     def OnProcessTool(self, event):
         eid = event.GetId()
         if eid == self.ID_ART_NATIVE:
             self.propgrid.SetArtProvider(pa.PropArtNative())
```

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/enumtype.py` & `bsmedit-3.2.9/bsmedit/propgrid/enumtype.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/formatters.py` & `bsmedit-3.2.9/bsmedit/propgrid/formatters.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/prop.py` & `bsmedit-3.2.9/bsmedit/propgrid/prop.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import traceback
 import copy
 import six
 import wx
 import wx.adv
 from .validators import *
 from .formatters import *
+from . import formatters as fmt
 from .enumtype import EnumType
+from .utility import PopupMenu
 
 wxEVT_PROP_SELECTED = wx.NewEventType()
 wxEVT_PROP_CHANGING = wx.NewEventType()
 wxEVT_PROP_CHANGED = wx.NewEventType()
 wxEVT_PROP_HIGHLIGHTED = wx.NewEventType()
 wxEVT_PROP_RIGHT_CLICK = wx.NewEventType()
 wxEVT_PROP_COLLAPSED = wx.NewEventType()
@@ -35,192 +37,242 @@
 EVT_PROP_KEYDOWN = wx.PyEventBinder(wxEVT_PROP_KEYDOWN, 1)
 EVT_PROP_RESIZE = wx.PyEventBinder(wxEVT_PROP_RESIZE, 1)
 EVT_PROP_REFRESH = wx.PyEventBinder(wxEVT_PROP_REFRESH, 1)
 EVT_PROP_DROP = wx.PyEventBinder(wxEVT_PROP_DROP, 1)
 EVT_PROP_BEGIN_DRAG = wx.PyEventBinder(wxEVT_PROP_BEGIN_DRAG, 1)
 
 
-class Property(object):
-    controls = EnumType('default', 'none', 'editbox', 'choice', 'file',
-                        'folder', 'slider', 'spin', 'checkbox', 'radiobox',
-                        'color', 'date', 'time', 'font')
+class PropBase():
+    pass
 
-    def __init__(self, grid, name, label, value):
-        self.grid = grid
-        self.name = name
+class PropGeneric(PropBase):
+    def __init__(self, label=''):
+        self.grid = None
+        self.name = ''
         self.label = label
         self.label_tip = ''
-        self.value = value
+        self.value = ''
         self.value_tip = ''
         # indicate if data is garbage
         self.value_valid = True
         # -1 to use the default one defined in parent's art provider
         self.title_width = -1
         self.indent = 0
         self.activated = False
         self.enable = True
         self.font_label = None
         self.font_value = None
         self.has_children = False
         self.expanded = True
         self.visible = True
         self.readonly = False
-        self.ctrl_type = self.controls.default
-        self.window = None
+        #self.window = None
         self.parent = -1
         self.SetTextColor(silent=True)
         self.SetBgColor(silent=True)
         self.min_size = wx.Size(200, 25)
         self.rect = wx.Rect(0, 0, 0, 0)
         # non-overlapping regions
         self.regions = {
             'value': wx.Rect(),
             'label': wx.Rect(),
             'splitter': wx.Rect(),
             'expander': wx.Rect()
         }
+        self.draws = {
+            'value': True,
+            'label': True,
+            'splitter': True,
+            'expander': True
+            }
         self.show_label_tips = False
         self.show_value_tips = False
         self.separator = False
         self.data = None
         self.formatter = None
 
+        self.draggable = True
+        self.configurable = True
+        self.top_value_border = False
+        self.bottom_value_border = False
+
+    def copy(self, p):
+        assert isinstance(p, PropGeneric)
+        self.grid = p.grid
+        if p.font_label:
+            self.font_label = wx.Font(p.font_label)
+        if p.font_value:
+            self.font_value = wx.Font(p.font_value)
+        self.SetTextColor(p.text_clr, p.text_clr_sel, p.text_clr_disabled, True)
+        self.SetBgColor(p.bg_clr, p.bg_clr_sel, p.bg_clr_disabled, True)
+        self.data = p.data
+        if p.formatter:
+            self.formatter = copy.copy(p.formatter)
+
+        self.name = p.name
+        self.label = p.label
+        self.label_tip = p.label_tip
+        self.value = p.value
+        self.value_tip = p.value_tip
+        # indicate if data is garbage
+        self.value_valid = p.value_valid
+        # -1 to use the default one defined in parent's art provider
+        self.title_width = p.title_width
+        self.indent = p.indent
+        self.activated = p.activated
+        self.enable = p.enable
+        self.visible = p.visible
+        self.readonly = p.readonly
+        self.min_size = p.min_size
+        self.draws = p.draws
+        self.show_label_tips = p.show_label_tips
+        self.show_value_tips = p.show_label_tips
+        self.separator = p.separator
+        self.data = copy.deepcopy(p.data)
+
+        self.draggable = p.draggable
+        self.configurable = p.configurable
+
     def duplicate(self):
         """
         copy the object
 
         copy.deepcopy does not work since the object contains pointer to wx
         objects
         """
-        p = Property(self.grid, self.name, self.label, self.value)
-        p.label_tip = self.label_tip
-        p.value_tip = self.value_tip
-        p.title_width = self.title_width
-        p.indent = self.indent
-        p.activated = self.activated
-        p.enable = self.enable
-        if p.font_label:
-            self.font_label = wx.Font(p.font_label)
-        if p.font_value:
-            self.font_value = wx.Font(p.font_value)
-        p.has_children = self.has_children
-        p.expanded = self.expanded
-        p.visible = self.visible
-        p.readonly = self.readonly
-        p.ctrl_type = self.ctrl_type
-        p.parent = self.parent
-        p.SetTextColor(self.text_clr, self.text_clr_sel,
-                       self.text_clr_disabled, True)
-        p.SetBgColor(self.bg_clr, self.bg_clr_sel, self.bg_clr_disabled, True)
-        p.show_label_tips = self.show_label_tips
-        p.show_value_tips = self.show_value_tips
-        p.separator = self.separator
-        p.data = self.data
-        p.formatter = copy.copy(p.formatter)
+        p = copy.copy(self)
+        p.copy(self)
         return p
 
+    def Grid(self, grid):
+        self.SetGrid(grid)
+        return self
+
     def SetGrid(self, grid):
         """set the grid window"""
         self.grid = grid
 
     def GetGrid(self):
         """return the grid window"""
         return self.grid
 
+    def Data(self, data):
+        self.SetData(data)
+        return self
+
     def SetData(self, data):
         self.data = data
 
     def GetData(self):
         return self.data
 
+    def Separator(self, sep=True, silent=True):
+        self.SetSeparator(sep, silent)
+        return self
+
     def SetSeparator(self, sep=True, silent=False):
         """set the property to be a separator"""
         if self.separator == sep:
             return
         self.separator = sep
         if not silent:
             self.Refresh()
 
     def IsSeparator(self):
         """return true if the property is a separator"""
         return self.separator
 
-    def SetControlStyle(self, style):
-        """set the control type
-        style: default | none | editbox | choice | file | folder | slider |
-               spin | checkbox | radiobox | color | date | time
-        """
-        self.UpdatePropValue()
-        self.DestroyControl()
-        if style not in self.controls:
-            print('Unsupported control style!')
-            return False
-        self.ctrl_type = self.controls[style]
-        return True
-
-    def GetControlStyle(self):
-        """return the control type"""
-        return self.ctrl_type
+    def Enable(self, enable=True, silent=True):
+        """enable/disable the property"""
+        self.SetEnable(enable, silent=silent)
+        return self
 
-    def Enable(self, enable=True, silent=False):
+    def SetEnable(self, enable=True, silent=False):
         """enable/disable the property"""
         if self.enable == enable:
             return
         self.enable = enable
         if not silent:
             self.Refresh()
 
     def IsEnabled(self):
         """return true if the property is enabled"""
         return self.enable
 
+    def Name(self, name, silent=True):
+        self.SetName(name, silent)
+        return self
+
     def SetName(self, name, silent=False):
         """set the name"""
         if self.name == name:
             return
         self.name = name
         if not silent:
             self.Refresh()
 
     def GetName(self):
         """get the name"""
         return self.name
 
+    def Label(self, label, silent=True):
+        self.SetLabel(label, silent)
+        return self
+
     def SetLabel(self, label, silent=False):
         """set the label"""
         if self.label == label:
             return
         self.label = label
+        if not self.name:
+            self.SetName(f'_prop_{label}', silent=True)
         if not silent:
             self.Refresh()
 
     def GetLabel(self):
         """get the label"""
         return self.label
 
+    def LabelTip(self, tip):
+        self.SetLabelTip(tip)
+        return self
+
     def SetLabelTip(self, tip):
         """set the label tip"""
         self.label_tip = tip
 
     def GetLabelTip(self):
         """get the label tip"""
         if self.label_tip:
             return self.label_tip
         return self.GetName()
 
+    def LabelFont(self, font, silent=False):
+        self.SetLabelFont(font, silent)
+        return self
+
     def SetLabelFont(self, font, silent=False):
         """set label font"""
         self.font_label = font
         if not silent:
             self.Refresh()
 
     def GetLabelFont(self):
         """get label font"""
         return self.font_label
 
+    def Visible(self, visible, silent=True):
+        """
+        show/hide the property
+
+        The property may be hidden if its parent is in collapsed mode.
+        """
+        self.SetVisible(visible, silent)
+        return self
+
     def SetVisible(self, visible=True, silent=False):
         """
         show/hide the property
 
         The property may be hidden if its parent is in collapsed mode.
         """
         if self.visible == visible:
@@ -229,30 +281,39 @@
         if not silent:
             self.Refresh(True)
 
     def IsVisible(self):
         """return true if the property is visible"""
         return self.visible
 
+    def Parent(self, prop):
+        """set the parent property"""
+        self.SetParent(prop)
+        return self
+
     def SetParent(self, prop):
         """set the parent property"""
         if prop and prop.GetIndent() >= self.GetIndent():
             return
         self.parent = prop
 
     def GetParent(self):
         """return the parent property"""
         return self.parent
 
+    def Value(self, value, silent=True):
+        """set the value"""
+        self.SetValue(value, silent)
+        return self
+
     def SetValue(self, value, silent=False):
         """set the value"""
         if self.IsReadonly():
             return False
         if self.value != value:
-            self.DestroyControl()
             fmt = self.formatter
             try:
                 if fmt and not fmt.validate(fmt.format(value)):
                     return False
             except:
                 traceback.print_exc(file=sys.stdout)
                 return False
@@ -273,83 +334,120 @@
                 # ignore format if data is not valid yet
                 return self.formatter.format(self.value)
         except:
             traceback.print_exc(file=sys.stdout)
 
         return str(self.value)
 
+    def ValueValid(self, valid):
+        """mark the value valid"""
+        self.SetValueValid(valid)
+        return self
+
     def SetValueValid(self, valid):
+        """mark the value valid"""
         self.value_valid = valid
 
     def GetValueValid(self):
+        """return if the value is valid"""
         return self.value_valid
 
+    def ValueTip(self, tip):
+        """set the value tip"""
+        self.SetValueTip(tip)
+        return self
+
     def SetValueTip(self, tip):
         """set the value tip"""
         self.value_tip = tip
 
     def GetValueTip(self):
         """get the valuetip"""
         if self.value_tip:
             return self.value_tip
         return self.GetValueAsString()
 
+    def ValueFont(self, font, silent=True):
+        """set value font"""
+        self.SetValueFont(font, silent)
+        return self
+
     def SetValueFont(self, font, silent=False):
         """set value font"""
         self.font_value = font
         if not silent:
             self.Refresh()
 
     def GetValueFont(self):
         """get value font"""
         return self.font_value
 
+    def Formatter(self, formatter):
+        """set value formatter"""
+        self.SetFormatter(formatter)
+        return self
+
     def SetFormatter(self, formatter):
+        """set value formatter"""
         if not formatter or not hasattr(formatter, 'validate') or\
            not hasattr(formatter, 'format') or not hasattr(formatter, 'coerce'):
             formatter = None
         self.formatter = formatter
 
     def GetFormatter(self):
+        """get value formatter"""
         return self.formatter
 
+    def Indent(self, indent, silent=True):
+        """set the indent to a positive integer"""
+        self.SetIndent(indent, silent)
+        return self
+
     def SetIndent(self, indent, silent=False):
         """set the indent to a positive integer"""
-        if indent < 0:
-            indent = 0
+        indent = max(indent, 0)
         if indent == self.indent:
             return
         self.indent = indent
         if not silent:
             self.SendPropEvent(wxEVT_PROP_INDENT)
 
     def GetIndent(self):
         """get the indent"""
         return self.indent
 
+    def Expand(self, expand=True, silent=True):
+        """expand/collapse the children"""
+        self.SetExpand(expand, silent)
+        return self
+
     def SetExpand(self, expand=True, silent=False):
         """expand/collapse the children"""
-        if not self.HasChildren():
-            return
         if expand == self.expanded:
             return
         self.expanded = expand
-        if silent:
+
+        if silent or not self.HasChildren():
             return
         if self.expanded:
             evt = wxEVT_PROP_EXPANDED
         else:
             evt = wxEVT_PROP_COLLAPSED
         if not silent:
             self.SendPropEvent(evt)
 
     def IsExpanded(self):
         """return true if the expand/collapse button is expanded"""
         return self.expanded
 
+    def Children(self, haschildren, silent=True):
+        """Indicate that the property has children"""
+        self.SetHasChildren(haschildren, silent)
+        return self
+
     def SetHasChildren(self, haschildren, silent=False):
         """Indicate that the property has children"""
         if haschildren == self.has_children:
             return
         self.has_children = haschildren
         if silent:
             return
@@ -359,40 +457,57 @@
             evt = wxEVT_PROP_COLLAPSED
         self.SendPropEvent(evt)
 
     def HasChildren(self):
         """return true if the property has children"""
         return self.has_children
 
+    def Activated(self, activated=True):
+        """activate the property"""
+        self.SetActivated(activated)
+        return self
+
     def SetActivated(self, activated=True):
         """activate the property"""
         if activated == self.activated:
             return
         self.activated = activated
-        if not activated:
-            # destroy the control if the property is inactivated
-            self.OnTextEnter()
-        else:
+        if activated:
             self.SendPropEvent(wxEVT_PROP_SELECTED)
 
     def IsActivated(self):
         """return true if the property is activated"""
         return self.activated
 
+    def Readyonly(self, readonly=True, silent=True):
+        """set the property to readonly"""
+        self.SetReadonly(readonly, silent)
+        return self
+
     def SetReadonly(self, readonly=True, silent=False):
         """set the property to readonly"""
         if readonly != self.IsReadonly():
             self.readonly = readonly
             if not silent:
                 self.Refresh()
 
     def IsReadonly(self):
         """return true if the property is readonly"""
         return self.readonly
 
+    def TextColor(self, clr=None, clr_sel=None, clr_disabled=None, silent=True):
+        """
+        set the text colors
+
+        All values are string. If the value is None, the color will reset to
+        default.
+        """
+        self.SetTextColor(clr, clr_sel, clr_disabled, silent)
+        return self
+
     def SetTextColor(self,
                      clr=None,
                      clr_sel=None,
                      clr_disabled=None,
                      silent=False):
         """
         set the text colors
@@ -407,14 +522,24 @@
         if not silent:
             self.Refresh()
 
     def GetTextColor(self):
         """get the text colors"""
         return (self.text_clr, self.text_clr_sel, self.text_clr_disabled)
 
+    def BgColor(self, clr=None, clr_sel=None, clr_disabled=None, silent=True):
+        """
+        set the background colors
+
+        All values are string. If the value is None, the color will reset to
+        default.
+        """
+        self.SetBgColor(clr, clr_sel, clr_disabled, silent)
+        return self
+
     def SetBgColor(self,
                    clr=None,
                    clr_sel=None,
                    clr_disabled=None,
                    silent=False):
         """
         set the background colors
@@ -429,62 +554,97 @@
         if not silent:
             self.Refresh()
 
     def GetBgColor(self):
         """get the background colors"""
         return (self.bg_clr, self.bg_clr_sel, self.bg_clr_disabled)
 
+    def TitleWidth(self, width):
+        """set the title width"""
+        self.SetTitleWidth(width)
+        return self
+
     def SetTitleWidth(self, width):
         """set the title width"""
         self.title_width = width
 
     def GetTitleWidth(self):
         """return the width"""
         return self.title_width
 
+    def Rect(self, rc):
+        """set the prop rect"""
+        self.SetRect(rc)
+        return self
+
     def SetRect(self, rc):
         """set the prop rect"""
         if self.rect != rc:
             self.rect = wx.Rect(*rc)
             # redraw the item
             self.Refresh()
-            wx.CallAfter(self.LayoutControl)
 
     def GetRect(self):
         """return the prop rect"""
         return wx.Rect(*self.rect)
 
+    def MinSize(self, size, silent=True):
+        """set the min size"""
+        self.SetMinSize(size, silent)
+        return self
+
     def SetMinSize(self, size, silent=False):
         """set the min size"""
         if self.min_size != size:
             self.min_size = wx.Size(*size)
             if not silent:
                 self.Resize()
 
     def GetMinSize(self):
         """return the min size"""
-        if self.window:
-            size = self.window.GetSize()
-            sz = self.min_size
-            size.y = max(sz.y, size.y)
-            return size
         return wx.Size(*self.min_size)
 
     def GetSize(self):
         """return the current size"""
         return self.rect.GetSize()
 
     def GetShowLabelTips(self):
         """return whether label tooltip is allowed"""
         return self.show_label_tips
 
     def GetShowValueTips(self):
         """return whether value tooltip is allowed"""
         return self.show_value_tips
 
+    def Draggable(self, draggable):
+        """set if it is allow to drag/drop the prop"""
+        self.SetDraggable(draggable)
+        return self
+
+    def SetDraggable(self, draggable):
+        """set if it is allow to drag/drop the prop"""
+        self.draggable = draggable
+
+    def IsDraggable(self):
+        """get if it is allow to drag/drop the prop"""
+        return self.draggable
+
+    def Configurable(self, configurable):
+        """set if it is allow to configure the prop"""
+        self.SetConfigurable(configurable)
+        return self
+
+    def SetConfigurable(self, configurable):
+        """set if it is allow to configure the prop"""
+        self.configurable = configurable
+
+    def IsConfigurable(self):
+        """get if it is allow to configure the prop"""
+        return self.configurable
+
     def HitTest(self, pt):
         """find the mouse position relative to the property"""
         # bottom edge
         rc = wx.Rect(*self.rect)
         rc.SetTop(rc.bottom - 2)
         if rc.Contains(pt):
             return 'bottom_edge'
@@ -502,358 +662,697 @@
 
     def OnMouseDown(self, pt):
         ht = self.HitTest(pt)
         # click on the expand buttons? expand it?
         if self.HasChildren() and ht == 'expander':
             self.SetExpand(not self.expanded)
 
-        if ht == 'value':
-            if not self.IsReadonly() and self.IsActivated():
-                self.CreateControl()
-        else:
-            self.UpdatePropValue()
-            self.DestroyControl()
-
         return ht
 
     def OnMouseUp(self, pt):
         ht = self.HitTest(pt)
         return ht
 
     def OnMouseDoubleClick(self, pt):
         ht = self.HitTest(pt)
 
         if self.IsEnabled():
-            if ht == 'value':
-                if not self.IsReadonly():
-                    self.CreateControl()
-            else:
-                self.UpdatePropValue()
-                self.DestroyControl()
-
             if ht == 'expander':
                 self.SetExpand(not self.expanded)
 
             self.SendPropEvent(wxEVT_PROP_DOUBLE_CLICK)
 
         return ht
 
     def OnMouseRightClick(self, pt):
         ht = self.HitTest(pt)
 
         if self.IsEnabled():
             # destroy the control when the mouse moves out
-            if ht is None:
-                self.UpdatePropValue()
-                self.DestroyControl()
             self.SendPropEvent(wxEVT_PROP_RIGHT_CLICK)
 
         return ht
 
     def OnMouseMove(self, pt):
         ht = self.HitTest(pt)
         return ht
 
-    def OnTextEnter(self):
-        self.UpdatePropValue()
+    def SendPropEvent(self, event):
+        """ send property grid event to parent"""
+        win = self.GetGrid()
+        evt = PropEvent(event, self)
+        evt.SetEventObject(win)
+        evt_handler = win.GetEventHandler()
+
+        if evt_handler.ProcessEvent(evt):
+            return not evt.GetVeto()
+        return False
+
+    def Resize(self):
+        """notify parent grid the size needs to be updated"""
+        self.SendPropEvent(wxEVT_PROP_RESIZE)
+
+    def Refresh(self, force=False):
+        """notify the parent to redraw the property"""
+        if self.IsVisible() or force:
+            self.SendPropEvent(wxEVT_PROP_REFRESH)
+
+    def PostRefresh(self):
+        pass
+
+class PropEvent(wx.PyCommandEvent):
+    def __init__(self, commandType, prop, id=0):
+        wx.PyCommandEvent.__init__(self, commandType, id)
+        self.prop = prop
+        self.veto = False
+
+    def GetProp(self):
+        """return the attached Property"""
+        return self.prop
+
+    def SetProp(self, prop):
+        """attach the Property instance"""
+        assert isinstance(prop, PropBase)
+        self.prop = prop
+
+    def Veto(self, veto=True):
+        """refuse the event"""
+        self.veto = veto
+
+    def GetVeto(self):
+        """return whether the event is refused"""
+        return self.veto
+
+class PropControl(PropGeneric):
+    def __init__(self, *args, **kwargs):
+        PropGeneric.__init__(self, *args, **kwargs)
+        self.window = None
+        self.allow_editing = True
+
+    def __del__(self):
         self.DestroyControl()
-        self.Refresh()
 
-    def CreateControl(self):
-        """create the control"""
-        if self.window != None or self.IsSeparator():
-            return
-        style = self.ctrl_type
-        if style == self.controls.default:
-            style = self.controls.editbox
-            if isinstance(self.formatter, EnumFormatter) or \
-               isinstance(self.formatter, ChoiceFormatter):
-                style = self.controls.choice
-            elif isinstance(self.formatter, BoolFormatter):
-                style = self.controls.checkbox
-            elif isinstance(self.formatter, PathFormatter):
-                if self.formatter.types == 'file':
-                    style = self.controls.file
-                elif self.formatter.types == 'folder':
-                    style = self.controls.folder
-            elif isinstance(self.formatter, ColorFormatter):
-                style = self.controls.color
-            elif isinstance(self.formatter, FontFormatter):
-                style = self.controls.font
-            elif isinstance(self.formatter, DateFormatter):
-                style = self.controls.date
-                if isinstance(self.formatter, TimeFormatter):
-                    style = self.controls.time
-        win = None
-        if style == self.controls.editbox:
-            style = wx.TE_PROCESS_ENTER
-            sz = self.GetMinSize()
-            if sz.y > 50:
-                style = wx.TE_MULTILINE
-            win = wx.TextCtrl(self.grid,
-                              wx.ID_ANY,
-                              self.GetValueAsString(),
-                              style=style)
-            if self.formatter:
-                validator = TextValidator(self, 'value', self.formatter, False,
-                                          None)
-                win.SetValidator(validator)
+    def Editing(self, enable):
+        self.SetEditting(enable)
+        return self
 
-            if style & wx.TE_PROCESS_ENTER:
-                win.Bind(wx.EVT_TEXT_ENTER, self.OnPropTextEnter)
+    def SetEditting(self, enable):
+        self.allow_editing = enable
 
-        elif style == self.controls.choice:
-            win = wx.Choice(self.grid, wx.ID_ANY)
-            if self.formatter:
-                validator = SelectorValidator(self, 'value', self.formatter,
-                                              True)
-                win.SetValidator(validator)
-
-        elif style == self.controls.file:
-            win = wx.Button(self.grid, wx.ID_ANY, self.GetValueAsString())
-            win.Bind(wx.EVT_BUTTON, self.OnSelectFile)
-
-        elif style == self.controls.folder:
-            win = wx.Button(self.grid, wx.ID_ANY, self.GetValueAsString())
-            win.Bind(wx.EVT_BUTTON, self.OnSelectFolder)
-
-        elif style == self.controls.slider:
-            win = wx.Slider(self.grid,
-                            wx.ID_ANY,
-                            value=int(self.value),
-                            style=wx.SL_LABELS | wx.SL_HORIZONTAL | wx.SL_TOP)
-            if self.formatter:
-                validator = SpinSliderValidator(self, 'value', self.formatter,
-                                                True)
-                win.SetValidator(validator)
-
-        elif style == self.controls.spin:
-            win = wx.SpinCtrl(self.grid,
-                              wx.ID_ANY,
-                              value=str(self.value),
-                              style=wx.SP_ARROW_KEYS)
-            if self.formatter:
-                validator = SpinSliderValidator(self, 'value', self.formatter,
-                                                True)
-                win.SetValidator(validator)
-
-        elif style == self.controls.checkbox:
-            win = wx.CheckBox(self.grid, wx.ID_ANY)
-            win.SetValue(int(self.value) != 0)
-
-        elif style == self.controls.radiobox:
-            choices = []
-            if self.formatter and hasattr(self.formatter, 'validValues'):
-                choices = [x[1] for x in self.formatter.validValues()]
+    def GetEditting(self):
+        return self.allow_editing
 
-            win = wx.RadioBox(self.grid, wx.ID_ANY, "", wx.DefaultPosition,
-                              wx.DefaultSize, choices, 5, wx.RA_SPECIFY_COLS)
+    def SetValue(self, value, silent=False):
+        self.DestroyControl()
+        return super().SetValue(value, silent)
 
-            if self.formatter:
-                validator = RadioBoxValidator(self, 'value', self.formatter,
-                                              True)
-                win.SetValidator(validator)
-
-        elif style == self.controls.color:
-            win = wx.ColourPickerCtrl(self.grid,
-                                      wx.ID_ANY,
-                                      wx.BLACK,
-                                      style=wx.CLRP_DEFAULT_STYLE
-                                      | wx.CLRP_SHOW_LABEL)
-            try:
-                win.SetColour(self.value)
-            except ValueError:
-                pass
-        elif style == self.controls.font:
-            win = wx.FontPickerCtrl(self.grid, wx.ID_ANY)
-            try:
-                if self.value:
-                    win.SetSelectedFont(self.value)
-            except ValueError:
-                pass
+    def SetActivated(self, activated=True):
+        """activate the property"""
+        super().SetActivated(activated)
+        if not activated:
+            # destroy the control if the property is inactivated
+            self.OnTextEnter()
 
-        elif style == self.controls.date:
-            win = wx.adv.DatePickerCtrl(self.grid, wx.ID_ANY)
-            try:
-                win.SetValue(self.value)
-            except ValueError:
-                pass
+    def SetRect(self, rc):
+        """set the prop rect"""
+        if self.rect != rc:
+            wx.CallAfter(self.LayoutControl)
+        super().SetRect(rc)
 
-        elif style == self.controls.time:
-            win = wx.adv.TimePickerCtrl(self.grid, wx.ID_ANY)
-            try:
-                win.SetValue(self.value)
-            except ValueError:
-                pass
-        if win:
+    def doCreateControl(self):
+        return None
+
+    def CreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return
+        if not self.allow_editing:
+            return
+        win = self.doCreateControl()
+
+        if win is not None:
             if win.GetValidator():
                 win.GetValidator().TransferToWindow()
             self.window = win
             # the window size may be larger than the value rect, notify parent
             # grid to update it
             self.Resize()
             self.LayoutControl()
             self.window.SetFocus()
-            self.window.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+            #self.window.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+            self.draws['value'] = False
+
+    def OnMouseDown(self, pt):
+        ht = super().OnMouseDown(pt)
+
+        if self.IsEnabled() and ht == 'value':
+            if not self.IsReadonly() and self.IsActivated():
+                self.CreateControl()
+        else:
+            self.UpdatePropValue()
+            self.DestroyControl()
+
+        return ht
+
+    def OnMouseDoubleClick(self, pt):
+        ht = self.HitTest(pt)
+
+        if self.IsEnabled():
+            if ht == 'value':
+                if not self.IsReadonly():
+                    self.CreateControl()
+            else:
+                self.UpdatePropValue()
+                self.DestroyControl()
+
+        return  super().OnMouseDoubleClick(pt)
+
+    def OnMouseRightClick(self, pt):
+        ht = self.HitTest(pt)
+
+        if self.IsEnabled():
+            # destroy the control when the mouse moves out
+            if ht is None:
+                self.UpdatePropValue()
+                self.DestroyControl()
+
+        return super().OnMouseRightClick(pt)
+
+    def OnTextEnter(self):
+        self.UpdatePropValue()
+        self.DestroyControl()
+        self.Refresh()
 
     def OnPropTextEnter(self, evt):
         """send when the enter key is pressed in the property control window"""
         if self.window:
             self.OnTextEnter()
 
-    def OnKillFocus(self, evt):
-        # destroy the control if it loses focus. Wait until the event has been
-        # processed; otherwise, it may crash.
-        evt.Skip()
-        wnd = evt.GetWindow()
-        while wnd:
-            if wnd.GetParent() == self.window:
-                return
-            wnd = wnd.GetParent()
-        # color window does not work on Mac
-        #wx.CallAfter(self.OnTextEnter)
+    def DestroyControl(self):
+        """destroy the value setting control"""
+        def _destroy():
+            if self.window:
+                self.window.Show(False)
+                self.window.Destroy()
+                self.window = None
+                self.Resize()
 
-    def OnSelectFile(self, evt):
-        style = wx.FD_OPEN | wx.FD_FILE_MUST_EXIST
-        dlg = wx.FileDialog(self.grid, "Choose a file",
-                            self.GetValueAsString(), "", "*.*", style)
-        if dlg.ShowModal() == wx.ID_OK:
-            self.SetValue(dlg.GetPath())
-        dlg.Destroy()
+        self.draws['value'] = True
+        if self.window:
+            # otherwise, it may crash (e..g, MacOS)
+            # not be able to reproduce it with MacOS 13.2.1
+            _destroy()
+            return True
+        return False
 
-    def OnSelectFolder(self, evt):
-        dlg = wx.DirDialog(self.grid, "Choose input directory",
-                           self.GetValueAsString(),
-                           wx.DD_DEFAULT_STYLE | wx.DD_DIR_MUST_EXIST)
-        if dlg.ShowModal() == wx.ID_OK:
-            self.SetValue(dlg.GetPath())
-        dlg.Destroy()
+    def doGetValueFromWin(self):
+        return None
+
+    def UpdatePropValue(self):
+        """update the value"""
+        if self.window is None:
+            return False
+        old_value = self.value
+        validator = self.window.GetValidator()
+        if validator:
+            validator.TransferFromWindow()
+        else:
+            value = self.doGetValueFromWin()
+            if value is not None:
+                value = self.coerce(value)
+            if value is not None:
+                self.SetValue(value, silent=True)
+        if old_value == self.value:
+            return False
+
+        if self.SendPropEvent(wxEVT_PROP_CHANGING):
+            self.SendPropEvent(wxEVT_PROP_CHANGED)
+            self.Refresh()
+            return True
+        else:
+            #the parent rejects the operation, restore the original value
+            self.SetValue(old_value)
+            return False
+        return False
 
     def LayoutControl(self):
         """re-positioning the control"""
         if self.window is None:
             return
         rc = self.grid.GetScrolledRect(wx.Rect(*self.regions['value']))
         self.window.SetSize(rc.GetSize())
         self.window.Move(rc.GetTopLeft())
 
-    def DestroyControl(self):
-        """destroy the value setting control"""
+    def GetMinSize(self):
+        """return the min size"""
         if self.window:
-            self.window.Show(False)
-            self.window.Destroy()
-            self.window = None
-            self.Resize()
-            return True
-        return False
+            size = self.window.GetSize()
+            sz = self.min_size
+            size.y = max(sz.y, size.y)
+            return size
+        return super().GetMinSize()
 
-    def UpdatePropValue(self):
+    def coerce(self, value):
+        try:
+            if self.formatter:
+                if self.formatter.validate(str(value)):
+                    value = self.formatter.coerce(str(value))
+                else:
+                    return None
+            elif self.value is not None:
+                value = type(self.value)(value)
+            return value
+        except ValueError:
+            traceback.print_exc(file=sys.stdout)
+            return None
+
+    def PostRefresh(self):
+        """notify the window to redraw itself"""
+        if self.window is not None:
+            self.window.Refresh()
+
+class PropSeparator(PropGeneric):
+    def __init__(self, *args, **kwargs):
+        PropGeneric.__init__(self, *args, **kwargs)
+        self.regions = {
+                'label': wx.Rect(),
+                'expander': wx.Rect()
+                }
+        self.draws = {
+                'value': False,
+                'label': True,
+                'splitter': False,
+                'expander': True
+                }
+        self.Separator(True)
+
+class PropEditBox(PropControl):
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        style = wx.TE_PROCESS_ENTER
+        sz = self.GetMinSize()
+        if sz.y > 50:
+            style = wx.TE_MULTILINE
+        win = wx.TextCtrl(self.grid, wx.ID_ANY, self.GetValueAsString(),
+                          style=style)
+        if self.formatter:
+            validator = TextValidator(self, 'value', self.formatter, False, None)
+            win.SetValidator(validator)
+            if style & wx.TE_PROCESS_ENTER:
+                win.Bind(wx.EVT_TEXT_ENTER, self.OnPropTextEnter)
+
+        return win
+
+    def OnPropTextEnter(self, evt):
+        """send when the enter key is pressed in the property control window"""
+        if self.window:
+            self.OnTextEnter()
+
+    def doGetValueFromWin(self):
         """update the value"""
         if self.window is None:
-            return False
-        validator = self.window.GetValidator()
-        if validator:
-            validator.TransferFromWindow()
-            return
+            return None
 
-        value_old = self.value
         value = None
         if isinstance(self.window, wx.TextCtrl):
             value = self.window.GetValue()
 
-        elif isinstance(self.window, wx.Button):
-            value = self.window.GetLabel()
+        return value
 
-        elif isinstance(self.window, wx.RadioBox) or\
-             isinstance(self.window, wx.Choice):
-            sel = self.window.GetSelection()
-            if sel >= 0 and sel < self.window.GetCount():
-                value = self.window.GetString(sel)
+class PropText(PropEditBox):
+    pass
 
-        elif isinstance(self.window, wx.Slider):
-            value = self.window.GetValue()
+class PropInt(PropText):
+    def __init__(self, *args, **kwargs):
+        PropText.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.IntFormatter())
+
+class PropHex(PropText):
+    def __init__(self, *args, **kwargs):
+        PropText.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.HexFormatter())
+
+class PropBin(PropText):
+    def __init__(self, *args, **kwargs):
+        PropText.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.BinFormatter())
+
+class PropFloat(PropText):
+    def __init__(self, *args, **kwargs):
+        PropText.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.FloatFormatter())
+
+class PropChoice(PropControl):
+    def __init__(self, choice, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.ChoiceFormatter(choice))
 
-        elif isinstance(self.window, wx.SpinCtrl):
-            value = self.window.GetValue()
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.Choice(self.grid, wx.ID_ANY)
+        if self.formatter:
+            validator = SelectorValidator(self, 'value', self.formatter, True)
+            win.SetValidator(validator)
 
-        elif isinstance(self.window, wx.CheckBox):
-            value = self.window.GetValue()
+        return win
 
-        elif isinstance(self.window, wx.ColourPickerCtrl):
-            clr = self.window.GetColour()
-            value = clr.GetAsString(wx.C2S_HTML_SYNTAX)
-
-        elif isinstance(self.window, wx.FontPickerCtrl):
-            font = self.window.GetSelectedFont()
-            value = font.GetNativeFontInfoDesc()
+    def doGetValueFromWin(self):
+        """update the value"""
+        if self.window is None:
+            return None
 
-        elif isinstance(self.window, wx.adv.DatePickerCtrl) or\
-             isinstance(self.window, wx.adv.TimePickerCtrl):
-            value = self.window.GetValue()
-            if self.formatter:
-                value = self.formatter.format(value)
+        sel = self.window.GetSelection()
+        if sel >= 0 and sel < self.window.GetCount():
+            value = self.window.GetString(sel)
+
+        return value
+
+
+class PropRadioBox(PropControl):
+    def __init__(self, choice=None, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        if choice is None:
+            choice = []
+        self.Formatter(fmt.ChoiceFormatter(choice))
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        choices = []
+        if self.formatter and hasattr(self.formatter, 'validValues'):
+            choices = [x[1] for x in self.formatter.validValues()]
+
+        win = wx.RadioBox(self.grid, wx.ID_ANY, "", wx.DefaultPosition,
+                          wx.DefaultSize, choices, 5, wx.RA_SPECIFY_COLS)
+
+        if self.formatter:
+            validator = RadioBoxValidator(self, 'value', self.formatter,
+                                          True)
+            win.SetValidator(validator)
+        return win
+
+    def doGetValueFromWin(self):
+        """update the value"""
+        if self.window is None:
+            return None
+        sel = self.window.GetSelection()
+        if sel >= 0 and sel < self.window.GetCount():
+            value = self.window.GetString(sel)
+            return value
+        return None
+
+class PropCheckBox(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.BoolFormatter())
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.CheckBox(self.grid, wx.ID_ANY)
+        win.SetValue(int(self.value) != 0)
+        return win
+
+    def doGetValueFromWin(self):
+        value = self.window.GetValue()
+        return value
+
+
+class PropFile(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.PathFormatter(False, 'file'))
+        self.selected_file = None
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        #win = wx.Button(self.grid, wx.ID_ANY, self.GetValueAsString())
+        #win.Bind(wx.EVT_BUTTON, self.OnSelectFile)
+        self.selected_file = None
+        self.doSelectFile()
+        return None
+
+    def doSelectFile(self):
+        style = wx.FD_OPEN | wx.FD_FILE_MUST_EXIST
+        dlg = wx.FileDialog(self.grid, "Choose a file",
+                            self.GetValueAsString(), "", "*.*", style)
+        if dlg.ShowModal() == wx.ID_OK:
+            self.SetValue(dlg.GetPath())
+        dlg.Destroy()
+
+    def doGetValueFromWin(self):
+        return self.selected_file
+
+class PropFolder(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.PathFormatter(False, 'folder'))
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        self.doSelectFolder()
+        return None
+
+    def doSelectFolder(self):
+        dlg = wx.DirDialog(self.grid, "Choose input directory",
+                           self.GetValueAsString(),
+                           wx.DD_DEFAULT_STYLE | wx.DD_DIR_MUST_EXIST)
+        if dlg.ShowModal() == wx.ID_OK:
+            self.SetValue(dlg.GetPath())
+        dlg.Destroy()
+
+class PropSpin(PropControl):
+    def __init__(self, min_value=0, max_value=2**31-1, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.IntFormatter(min_value, max_value))
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.SpinCtrl(self.grid,
+                          wx.ID_ANY,
+                          value=str(self.value),
+                          style=wx.SP_ARROW_KEYS)
+        if self.formatter:
+            validator = SpinSliderValidator(self, 'value', self.formatter,
+                                            True)
+            win.SetValidator(validator)
+        return win
+
+    def doGetValueFromWin(self):
+        """update the value"""
+        if self.window is None:
+            return None
+        value = self.window.GetValue()
+
+        return value
+
+class PropSlider(PropControl):
+    def __init__(self, min_value=0, max_value=2**31-1, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.Formatter(fmt.IntFormatter(min_value, max_value))
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.Slider(self.grid,
+                        wx.ID_ANY,
+                        value=int(self.value),
+                        style=wx.SL_LABELS | wx.SL_HORIZONTAL | wx.SL_TOP)
+        if self.formatter:
+            validator = SpinSliderValidator(self, 'value', self.formatter,
+                                            True)
+            win.SetValidator(validator)
+        return win
+
+    def doGetValueFromWin(self):
+        if self.window is None:
+            return None
+        value = self.window.GetValue()
+        return value
+
+class PropDate(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.SetFormatter(fmt.DateFormatter())
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.adv.DatePickerCtrl(self.grid, wx.ID_ANY)
         try:
-            if self.formatter:
-                if self.formatter.validate(str(value)):
-                    value = self.formatter.coerce(str(value))
-                else:
-                    return False
-            elif self.value is not None:
-                value = type(self.value)(value)
-            self.SetValue(value, silent=True)
+            win.SetValue(self.value)
         except ValueError:
-            traceback.print_exc(file=sys.stdout)
-            return False
+            pass
+        return win
 
-        if self.SendPropEvent(wxEVT_PROP_CHANGING):
-            self.SendPropEvent(wxEVT_PROP_CHANGED)
+    def doGetValueFromWin(self):
+        if self.window is None:
+            return None
+        value = self.window.GetValue()
+        if self.formatter:
+            value = self.formatter.format(value)
+
+        return value
+
+class PropTime(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.SetFormatter(fmt.TimeFormatter())
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        win = wx.adv.TimePickerCtrl(self.grid, wx.ID_ANY)
+        try:
+            win.SetValue(self.value)
+        except ValueError:
+            pass
+        return win
+
+    def doGetValueFromWin(self):
+        if self.window is None:
+            return None
+        value = self.window.GetValue()
+        if self.formatter:
+            value = self.formatter.format(value)
+
+        return value
+
+class PropDateTime(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.SetFormatter(fmt.DateTimeFormatter())
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        menu = wx.Menu()
+        date = menu.Append(wx.ID_ANY, 'Update date')
+        time = menu.Append(wx.ID_ANY, 'Update time')
+        cmd = PopupMenu(self.grid, menu)
+        win = None
+        if cmd == time.GetId():
+            win = wx.adv.TimePickerCtrl(self.grid, wx.ID_ANY)
+        elif cmd == date.GetId():
+            win = wx.adv.DatePickerCtrl(self.grid, wx.ID_ANY)
+        if win is not None:
+            try:
+                win.SetValue(self.value)
+            except ValueError:
+                pass
+        return win
+
+    def doGetValueFromWin(self):
+        if self.window is None:
+            return None
+        value = self.window.GetValue()
+        if self.formatter:
+            value = self.formatter.format(value)
+
+        return value
+
+class PropFont(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.SetFormatter(fmt.FontFormatter())
+
+        self.auto_apply = True
+
+    def AutoApply(self, apply):
+        self.SetAutoApply(apply, True)
+
+    def SetAutoApply(self, apply, silent=False):
+        self.auto_apply = apply
+        if not silent:
             self.Refresh()
-            return True
-        else:
-            #the parent rejects the operation, restore the original value
-            self.SetValue(value_old)
-            return False
 
-    def SendPropEvent(self, event):
-        """ send property grid event to parent"""
-        win = self.GetGrid()
-        evt = PropertyEvent(event)
-        evt.SetProperty(self)
-        evt.SetEventObject(win)
-        evt_handler = win.GetEventHandler()
+    def GetAutoApply(self):
+        return self.auto_apply
 
-        if evt_handler.ProcessEvent(evt):
-            return not evt.GetVeto()
-        return False
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
 
-    def Resize(self):
-        """notify parent grid the size needs to be updated"""
-        self.SendPropEvent(wxEVT_PROP_RESIZE)
+        data = wx.FontData()
+        data.SetInitialFont(wx.Font(self.GetValue()))
+        dlg = wx.FontDialog(self.grid, data)
+        if dlg.ShowModal() == wx.ID_OK:
+            self.SetValue(dlg.GetFontData().GetChosenFont())
+        return None
 
-    def Refresh(self, force=False):
-        """notify the parent to redraw the property"""
-        if self.IsVisible() or force:
-            self.SendPropEvent(wxEVT_PROP_REFRESH)
+    def SetValue(self, value, silent=False):
+        if isinstance(value, wx.Font):
+            value = value.GetNativeFontInfoDesc()
 
+        if super().SetValue(value, True):
+            if self.auto_apply:
+                # set the font for value
+                font = wx.Font(self.GetValue())
+                font.SetFractionalPointSize(wx.NORMAL_FONT.GetFractionalPointSize())
+                self.SetValueFont(font, True)
+            if not silent:
+                self.Refresh()
 
-class PropertyEvent(wx.PyCommandEvent):
-    def __init__(self, commandType, id=0):
-        wx.PyCommandEvent.__init__(self, commandType, id)
-        self.prop = None
-        self.veto = False
+    def GetValueAsString(self):
+        """get the value as string"""
+        font =  wx.Font(self.GetValue())
+        return f'{font.GetFaceName()}, {font.GetFractionalPointSize()}'
 
-    def GetProperty(self):
-        """return the attached Property"""
-        return self.prop
+class PropColor(PropControl):
+    def __init__(self, *args, **kwargs):
+        PropControl.__init__(self, *args, **kwargs)
+        self.SetFormatter(fmt.ColorFormatter())
+        self.auto_apply = True
 
-    def SetProperty(self, prop):
-        """attach the Property instance"""
-        if isinstance(prop, Property):
-            self.prop = prop
+    def AutoApply(self, apply):
+        self.SetAutoApply(apply, True)
 
-    def Veto(self, veto=True):
-        """refuse the event"""
-        self.veto = veto
+    def SetAutoApply(self, apply, silent=False):
+        self.auto_apply = apply
+        if not silent:
+            self.Refresh()
 
-    def GetVeto(self):
-        """return whether the event is refused"""
-        return self.veto
+    def GetAutoApply(self):
+        return self.auto_apply
+
+    def doCreateControl(self):
+        """create the control"""
+        if self.window is not None:
+            return self.window
+        data = wx.ColourData()
+        data.SetColour(wx.Colour(self.GetValue()))
+        dlg = wx.ColourDialog(self.grid, data)
+        if dlg.ShowModal() == wx.ID_OK:
+            self.SetValue(dlg.GetColourData().GetColour())
+        return None
+
+    def SetValue(self, value, silent=False):
+        if isinstance(value, wx.Colour):
+            value = value.GetAsString(wx.C2S_HTML_SYNTAX)
+        if super().SetValue(value, True):
+            if self.auto_apply:
+                t = wx.Colour(self.GetValue())
+                c = t.GetAsString(wx.C2S_HTML_SYNTAX)
+                self.SetBgColor(c, c, c, True)
+                t.SetRGB(t.GetRGB() ^ 0xFFFFFF)
+                t = t.GetAsString(wx.C2S_HTML_SYNTAX)
+                self.SetTextColor(t, t, t, True)
+
+            if not silent:
+                self.Refresh()
```

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/propart.py` & `bsmedit-3.2.9/bsmedit/propgrid/propart.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,20 +102,22 @@
         if self.expansion_width > 0 and p.HasChildren():
             # expander icon
             rc = wx.Rect(*irc)
             rc.x = x + mx
             rc.SetWidth(self.expansion_width)
             p.regions['expander'] = rc
             x = rc.right
+        else:
+            p.regions['expander'] = wx.Rect(irc.right, irc.top, 0, 0)
 
         # label
         p.regions['label'] = wx.Rect(*irc)
         p.regions['label'].x = x + mx * 2
 
-        if not p.IsSeparator():
+        if 'value' in p.regions:
             title_width = p.title_width
             if title_width < 0:
                 title_width = self.title_width
             p.regions['label'].SetRight(title_width)
             x = p.regions['label'].right
 
             rc = wx.Rect(*irc)
@@ -125,19 +127,18 @@
             x = rc.right
 
             rc = wx.Rect(*irc)
             rc.x = x
             rc.SetWidth(irc.right - x)
             p.regions['value'] = rc
         else:
+            pass
             # separator does not have splitter & value
-            p.regions['label'].SetWidth(p.regions['label'].GetWidth() +
-                                        irc.right - x)
-            p.regions['splitter'] = wx.Rect(irc.right, irc.top, 0, 0)
-            p.regions['value'] = wx.Rect(irc.right, irc.top, 0, 0)
+            #p.regions['splitter'] = wx.Rect(irc.right, irc.top, 0, 0)
+            #p.regions['value'] = wx.Rect(irc.right, irc.top, 0, 0)
 
     def DrawSplitter(self, dc, p):
         # draw splitter
         rcs = p.regions['splitter']
         dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
         dc.DrawLine(rcs.left, rcs.top, rcs.left, rcs.bottom)
         dc.DrawLine(rcs.right - 1, rcs.top, rcs.right - 1, rcs.bottom)
@@ -171,15 +172,16 @@
         if p.font_value is None:
             font = self._font_value
         else:
             font = wx.Font(p.font_value)
         dc.SetFont(font)
 
         p.show_value_tips = False
-        if p.window is None:
+
+        if p.draws.get('value', False):
             crbg = p.bg_clr
             crtxt = wx.BLACK
             if not p.IsEnabled() or p.IsReadonly():
                 crtxt = p.text_clr_disabled
                 if not crtxt:
                     crtxt = self.text_clr_disabled
                 crbg = p.bg_clr_disabled
@@ -236,53 +238,80 @@
         bg = p.GetGrid().GetBackgroundColour()
         pen = wx.Pen(wx.BLACK, 1, wx.PENSTYLE_TRANSPARENT)
         dc.SetPen(pen)
         brush = wx.Brush(bg)
         dc.SetBrush(brush)
         dc.DrawRectangle(rc.x, rc.y, rc.width, rc.height)
 
-        dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
-        dc.DrawLine(rc.left, rc.bottom, rc.right, rc.bottom)
-        dc.DrawLine(rc.left, rc.top, rc.left, rc.bottom)
-        dc.DrawLine(rc.right - 1, rc.top, rc.right - 1, rc.bottom)
-        dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DHILIGHT)))
-        dc.DrawLine(rc.left, rc.top, rc.right, rc.top)
-        dc.DrawLine(rc.left + 1, rc.top, rc.left + 1, rc.bottom)
-        dc.DrawLine(rc.right, rc.top, rc.right, rc.bottom)
-
     def DrawBorder(self, dc, p):
-        rc = p.GetRect()
+        def _draw_line(rc, top=True, bot=True):
+            # top & bottom border
+            if bot:
+                crbg = self.bg_clr
+                if p.IsEnabled() and not p.IsReadonly():
+                    crbg = self.bg_clr_disabled
+                else:
+                    crbg = self.bg_clr
+                dc.SetPen(wx.Pen(wx.Colour(crbg)))
+                dc.DrawLine(rc.left, rc.bottom, rc.right, rc.bottom)
 
-        # top & bottom border
-        dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)))
-        dc.DrawLine(rc.left, rc.bottom, rc.right, rc.bottom)
-        dc.DrawLine(rc.left, rc.top, rc.left, rc.bottom)
-        dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DHILIGHT)))
-        dc.DrawLine(rc.left, rc.top, rc.right, rc.top)
-        dc.DrawLine(rc.left + 1, rc.top, rc.left + 1, rc.bottom)
+                clr = wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DSHADOW)
+                dc.SetPen(wx.Pen(clr))
+                #dc.SetPen(wx.Pen(wx.RED))
+                dc.DrawLine(rc.left, rc.bottom, rc.right, rc.bottom)
+            #dc.DrawLine(rc.left, rc.top, rc.left, rc.bottom)
+            if top:
+                dc.SetPen(wx.Pen(wx.SystemSettings.GetColour(wx.SYS_COLOUR_3DHILIGHT)))
+                dc.DrawLine(rc.left, rc.top, rc.right, rc.top)
+            #dc.DrawLine(rc.left + 1, rc.top, rc.left + 1, rc.bottom)
 
+        rc = p.GetRect()
+        rcs = p.regions.get('splitter', None)
+        if rcs is not None and rcs.width > 0:
+            rc.right = rcs.left
+            _draw_line(rc)
+            rc = p.GetRect()
+            rc.left = rcs.right
+            if p.top_value_border:
+                _draw_line(rc, top=p.top_value_border, bot=p.bottom_value_border)
+            if not p.bottom_value_border:
+                crbg = p.bg_clr
+                if p.IsEnabled() and not p.IsReadonly():
+                    crbg = p.bg_clr_disabled
+                    if not crbg:
+                        crbg = self.bg_clr_disabled
+                else:
+                    crbg = p.bg_clr
+                    if not crbg:
+                        crbg = self.bg_clr
+
+                dc.SetPen(wx.Pen(wx.Colour(crbg)))
+                dc.DrawLine(rc.left, rc.bottom, rc.right, rc.bottom)
+        else:
+            _draw_line(rc)
         # draw selected box
         if p.activated:
             dc.SetPen(wx.Pen(wx.BLACK, 1, wx.PENSTYLE_DOT))
             dc.SetBrush(wx.Brush(wx.BLACK, wx.BRUSHSTYLE_TRANSPARENT))
             dc.DrawRectangle(p.GetRect())
 
     def DrawItem(self, dc, p):
         """draw the property"""
         if not p.IsVisible():
             return
 
         dc.SetBackgroundMode(wx.TRANSPARENT)
+        dc.DestroyClippingRegion()
 
         self.PrepareDrawRect(p)
 
         self.DrawBackground(dc, p)
 
         self.DrawExpansion(dc, p)
         self.DrawLabel(dc, p)
-
         # separator does not have radio button, splitter bar and value sections
-        if not p.IsSeparator():
-            self.DrawSplitter(dc, p)
+        if 'value' in p.regions:
             self.DrawValue(dc, p)
 
         self.DrawBorder(dc, p)
+        if 'value' in p.regions:
+            self.DrawSplitter(dc, p)
```

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/propgrid.py` & `bsmedit-3.2.9/bsmedit/propgrid/propgrid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,50 @@
 import sys
 import traceback
-import json
 import six
 import wx
 import wx.py.dispatcher as dp
-import wx.lib.agw.aui as aui
 from .prop import *
-from .formatters import *
 from .propart import PropArtNative
+from .utility import PopupMenu
 
 wxEVT_PROP_INSERT = wx.NewEventType()
 wxEVT_PROP_DELETE = wx.NewEventType()
 
 EVT_PROP_INSERT = wx.PyEventBinder(wxEVT_PROP_INSERT, 1)
 EVT_PROP_DELETE = wx.PyEventBinder(wxEVT_PROP_DELETE, 1)
 
-
-def PopupMenu(wnd, menu):
-    if not wnd or not menu:
-        return wx.ID_NONE
-
-    cc = aui.ToolbarCommandCapture()
-    wnd.PushEventHandler(cc)
-
-    wnd.PopupMenu(menu)
-
-    command = cc.GetCommandId()
-    wnd.PopEventHandler(True)
-    return command
-
-
 class PropDropTarget(wx.DropTarget):
     def __init__(self, frame):
         wx.DropTarget.__init__(self)
         self.obj = wx.TextDataObject()
         self.SetDataObject(self.obj)
         self.frame = frame
+        self.SetDefaultAction(wx.DragMove)
 
     def OnEnter(self, x, y, d):
-        return super(PropDropTarget, self).OnDragOver(x, y, d)
+        self.frame.OnEnter(x, y, d)
+        return d
 
     def OnLeave(self):
-        pass
+        self.frame.OnLeave()
+
+    def OnDrop(self, x, y):
+        return True
 
     def OnData(self, x, y, d):
         if not self.GetData():
             return wx.DragNone
         self.frame.OnDrop(x, y, self.obj.GetText())
 
         return d
 
     def OnDragOver(self, x, y, d):
-        pt = wx.Point(x, y)
-        rc = self.frame.GetClientRect()
-        if rc.Contains(pt):
-            (x, y) = self.frame.GetViewStart()
-            if pt.y < 15:
-                self.frame.Scroll(-1, y - (15 - pt.y) / 3)
-            if pt.y > rc.bottom - 15:
-                self.frame.Scroll(-1, y - (rc.bottom - 15 - pt.y) / 3)
-        return super(PropDropTarget, self).OnDragOver(x, y, d)
+        self.frame.OnDragOver(x, y, d)
+        return d
 
 
 class PropGrid(wx.ScrolledWindow):
     ID_PROP_GRID_ADD_SEP = wx.NewId()
     ID_PROP_GRID_READ_ONLY = wx.NewId()
     ID_PROP_GRID_INDENT_INS = wx.NewId()
     ID_PROP_GRID_INDENT_DES = wx.NewId()
@@ -83,18 +64,17 @@
 
     SCROLL_UNIT = 15
 
     CURSOR_RESIZE_HORZ = 0
     CURSOR_RESIZE_VERT = 1
     CURSOR_STD = 2
 
-    def __init__(self, frame, prop_cls=Property):
+    def __init__(self, frame):
         wx.ScrolledWindow.__init__(self, frame)
 
-        self._prop_cls = prop_cls
         self.prop_selected = None
         self.cursor_mode = self.CURSOR_STD
         self.pos_mouse_down = wx.Point(0, 0)
         self.prop_under_mouse = None
         self.resize_mode = self.RESIZE_NONE
 
         self._props = []
@@ -105,27 +85,33 @@
         self.resize_cursor_vert = wx.Cursor(wx.CURSOR_SIZENS)
 
         # set scroll parameters
         self.SetScrollRate(self.SCROLL_UNIT, self.SCROLL_UNIT)
         self.SetVirtualSize(wx.Size(100, 200))
 
         self.SetDropTarget(PropDropTarget(self))
+        self.draggable = True
+        self.configurable = True
+
+        self.drag_image = None
+        self.drag_bitmap = None
 
         self.Bind(wx.EVT_PAINT, self.OnPaint)
         self.Bind(wx.EVT_SIZE, self.OnSize)
         self.Bind(wx.EVT_ERASE_BACKGROUND, self.OnEraseBackground)
         self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
         self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
         self.Bind(wx.EVT_RIGHT_DOWN, self.OnMouseRightClick)
         self.Bind(wx.EVT_LEFT_DCLICK, self.OnMouseDoubleClick)
         self.Bind(wx.EVT_MOTION, self.OnMouseMove)
         self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
         self.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
         # calling CaptureMouse requires to implement EVT_MOUSE_CAPTURE_LOST
         self.Bind(wx.EVT_MOUSE_CAPTURE_LOST, self.OnMouseCaptureLost)
+        self.Bind(wx.EVT_MOUSE_CAPTURE_CHANGED, self.OnMouseCaptureLost)
 
         self.Bind(EVT_PROP_SELECTED, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_CHANGING, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_CHANGED, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_HIGHLIGHTED, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_RIGHT_CLICK, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_COLLAPSED, self.OnPropEventsHandler)
@@ -136,150 +122,187 @@
         self.Bind(EVT_PROP_RESIZE, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_REFRESH, self.OnPropRefresh)
         self.Bind(EVT_PROP_DROP, self.OnPropEventsHandler)
         self.Bind(EVT_PROP_BEGIN_DRAG, self.OnPropEventsHandler)
         self.Bind(wx.EVT_MENU, self.OnProcessCommand)
         self.SetBackgroundStyle(wx.BG_STYLE_PAINT)
 
+    def CreateDragImage(self, prop):
+        memory = wx.MemoryDC(wx.Bitmap(1, 1))
+
+        w, h = prop.GetSize()
+        w = min(500, w-100)
+
+        scale_factor = self.GetContentScaleFactor()
+        bitmap = wx.Bitmap(w*scale_factor, h*scale_factor)
+        bitmap.SetScaleFactor(scale_factor)
+        memory.SelectObject(bitmap)
+
+        memory.Clear()
+        p = prop.duplicate()
+        p.SetGrid(self)
+        p.top_value_border = True
+        p.bottom_value_border = True
+        p.activated = True
+        p.SetRect(wx.Rect(0, 0, w, h))
+        self._art.DrawItem(memory, p)
+
+        memory.SelectObject(wx.NullBitmap)
+
+        return bitmap
+
     def SetArtProvider(self, art):
         self._art = art
         self.Refresh()
 
     def GetArtProvider(self):
         return self._art
 
-    def AppendProperty(self, name, label="", value="", update=True):
-        return self.InsertProperty(name, label, value, -1, update)
+    def Draggable(self, draggable):
+        """set if it is allow to drag/drop any prop"""
+        self.SetDraggable(draggable)
+        return self
+
+    def SetDraggable(self, draggable):
+        """set if it is allow to drag/drop any prop"""
+        self.draggable = draggable
+
+    def IsDraggable(self):
+        """get if it is allow to drag/drop any prop"""
+        return self.draggable
+
+    def Configurable(self, configurable):
+        """set if it is allow to drag/drop any prop"""
+        self.SetConfigurable(configurable)
+        return self
+
+    def SetConfigurable(self, configurable):
+        """set if it is allow to drag/drop any prop"""
+        self.configurable = configurable
+
+    def IsConfigurable(self):
+        """get if it is allow to drag/drop any prop"""
+        return self.configurable
+
+    def Append(self, prop, update=True):
+        return self.Insert(prop, -1, update)
 
-    def _InsertProperty(self, prop, index=-1, update=True):
+    def Insert(self, prop, index=-1, update=True):
         # add the prop window to the grid
-        if not isinstance(prop, Property):
+        if not isinstance(prop, PropBase):
             return None
 
-        if index == -1 or index >= self.GetPropCount():
+        prop.Grid(self)
+        if index == -1 or index >= self.GetCount():
             self._props.append(prop)
         else:
             self._props.insert(index, prop)
         name = prop.GetName()
 
         if index != -1 and (not update):
             self.CheckProp()
         if update:
             self.UpdateGrid()
         if self.SendPropEvent(wxEVT_PROP_INSERT, prop):
             dp.send('prop.insert', prop=prop)
         return prop
 
-    def InsertProperty(self, name, label="", value="", index=-1, update=True):
-        # add the prop window to the grid
-        prop = self._prop_cls(self, name, label, value)
-        return self._InsertProperty(prop, index, update)
-
-    def CopyProperty(self, prop, index=-1, update=True):
-        if not isinstance(prop, Property):
+    def CopyProp(self, prop, index=-1, update=True):
+        if not isinstance(prop, PropBase):
             return None
         p = prop.duplicate()
-        p.SetParent(self)
-        return self._InsertProperty(p, index, update)
+        p.SetGrid(self)
+        p.Activated(False)
+        return self.Insert(p, index, update)
 
-    def InsertSeparator(self,
-                        name='Separator',
-                        label='',
-                        index=-1,
-                        update=True):
-        prop = self.InsertProperty(name, label, '', index, update)
-        if prop:
-            prop.SetSeparator(True)
-        return prop
-
-    def RemoveProperty(self, prop, update=True):
+    def Remove(self, prop, update=True):
         # remove property
-        if isinstance(prop, six.string_types) or isinstance(prop, Property):
-            index = self.FindPropertyIndex(prop)
+        if isinstance(prop, six.string_types) or isinstance(prop, PropBase):
+            index = self.Index(prop)
         elif isinstance(prop, int):
             index = prop
         else:
             return False
 
-        if index >= 0 and index < self.GetPropCount():
+        if index >= 0 and index < self.GetCount():
             prop = self._props[index]
             activated = False
             if prop == self.prop_selected:
                 activated = True
                 self.SetSelection(-1)
             del self._props[index]
 
             if index != -1 and (not update):
                 self.CheckProp()
-            if index >= self.GetPropCount():
-                index = self.GetPropCount() - 1
+            if index >= self.GetCount():
+                index = self.GetCount() - 1
 
             if activated:
                 self.SetSelection(index)
             if update:
                 self.UpdateGrid()
             return True
         return False
 
-    def DeleteAllProperties(self, update=True):
+    def DeleteAll(self, update=True):
         for i in range(len(self._props) - 1, -1, -1):
-            self.DeleteProperty(self._props[i], update)
+            self.Delete(self._props[i], update)
 
-    def DeleteProperty(self, prop, update=True):
+    def Delete(self, prop, update=True):
         if self.SendPropEvent(wxEVT_PROP_DELETE, prop):
             dp.send('prop.delete', prop=prop)
-            return self.RemoveProperty(prop, update)
+            return self.Remove(prop, update)
         else:
             return False
 
-    def FindPropertyIndex(self, prop):
+    def Index(self, prop):
         """return the index of prop, or -1 if not found"""
-        p = self.GetProperty(prop)
+        p = self.Get(prop)
         if not p:
             return -1
         try:
             idx = self._props.index(p)
             return idx
         except ValueError:
             traceback.print_exc(file=sys.stdout)
         return -1
 
-    def GetProperty(self, prop):
-        """return the Property instance"""
-        if isinstance(prop, Property):
+    def Get(self, prop):
+        """return the prop instance"""
+        if isinstance(prop, PropBase):
             # if prop is a Property instance, simply return
             return prop
         elif isinstance(prop, six.string_types):
             # search the prop name
             props = [p for p in self._props if p.GetName() == prop]
             if not props:
                 return None
             elif len(props) == 1:
                 return props[0]
             return props
         elif isinstance(prop, int):
             # prop is the index
             index = prop
-            if index >= 0 and index < self.GetPropCount():
+            if index >= 0 and index < self.GetCount():
                 return self._props[index]
         return None
 
-    def GetPropCount(self):
+    def GetCount(self):
         """return the number of properties"""
         return len(self._props)
 
     def GetScrolledRect(self, rc):
         (x, y) = self.GetViewStart()
         rcs = wx.Rect(*rc)
         rcs.Offset(wx.Point(-x * self.SCROLL_UNIT, -y * self.SCROLL_UNIT))
         return rcs
 
     def EnsureVisible(self, prop):
         """scroll the window to make sure prop is visible"""
-        p = self.GetProperty(prop)
+        p = self.Get(prop)
         if not p:
             return
         rc_prop = p.GetRect()
         # translate to the scrolled position
         rc_prop.x, rc_prop.y = self.CalcScrolledPosition(rc_prop.x, rc_prop.y)
         _, y = self.GetViewStart()
         rc = self.GetRect()
@@ -293,23 +316,23 @@
         elif rc.bottom < rc_prop.bottom:
             # if the prop is under bottom of the client window, scroll down
             y = y + ((rc_prop.bottom - rc.bottom) / self.SCROLL_UNIT)
             self.Scroll(-1, y)
 
     def GetSelection(self):
         """get the index of the selected property"""
-        return self.FindPropertyIndex(self.prop_selected)
+        return self.Index(self.prop_selected)
 
-    def GetSelectedProperty(self):
+    def GetSelected(self):
         """return the selected property"""
         return self.prop_selected
 
     def SetSelection(self, prop):
         """set the active property"""
-        p = self.GetProperty(prop)
+        p = self.Get(prop)
         if p != self.prop_selected:
             if self.prop_selected:
                 self.prop_selected.SetActivated(False)
             self.prop_selected = p
             if self.prop_selected:
                 self.prop_selected.SetActivated(True)
             self.Refresh()
@@ -319,44 +342,44 @@
     def UpdateGrid(self):
         """update the grid"""
         self.LayoutAll()
         self.Refresh()
 
     def MoveProperty(self, prop, step):
         """move the property"""
-        index = self.FindPropertyIndex(prop)
+        index = self.Index(prop)
         if index == -1:
             return
 
         if step == 0:
             # move zero step is no move at all
             return
 
         # calculate the new position
         index2 = index + step
         if index2 < 0:
             index2 = 0
         # move the prop, prop will be placed on top of index2
-        if index2 < self.GetPropCount():
+        if index2 < self.GetCount():
             self.doMoveProperty(index, index2)
         else:
             self.doMoveProperty(index, -1)
 
     def doMoveProperty(self, index, index2):
         """move the property"""
         # the same position, ignore it
         if index == index2:
             return
 
-        prop = self.GetProperty(index)
+        prop = self.Get(index)
         props = [prop]
         if prop.HasChildren() and (not prop.IsExpanded()):
             # move all the children if they are not visible
             indent = prop.GetIndent()
-            for i in six.moves.range(index + 1, self.GetPropCount()):
+            for i in six.moves.range(index + 1, self.GetCount()):
                 if self._props[i].GetIndent() <= indent:
                     break
                 props.append(self._props[i])
 
         i = 0
         for p in props:
             if index2 == -1:
@@ -390,21 +413,20 @@
         # here the step is -1. For example, prop is at position 5, to move it
         # to position 4, we can say move it in front of position 4. Delete the
         # original prop will not affect the position of the new copy.
         self.MoveProperty(prop, -1)
 
     def SendPropEvent(self, event, prop=None):
         """send the property event to the parent"""
-        prop = self.GetProperty(prop)
+        prop = self.Get(prop)
         # prepare the event
-        if isinstance(event, PropertyEvent):
+        if isinstance(event, PropEvent):
             evt = event
         elif isinstance(event, int):
-            evt = PropertyEvent(event)
-            evt.SetProperty(prop)
+            evt = PropEvent(event, prop)
         else:
             raise ValueError()
 
         evt.SetId(self.GetId())
         eventObject = self.GetParent()
         evt.SetEventObject(eventObject)
         evtHandler = eventObject.GetEventHandler()
@@ -418,15 +440,15 @@
         # find the next visible property and activate it
         while True:
             if down:
                 sel += 1
             else:
                 sel -= 1
 
-            if sel < 0 or sel >= self.GetPropCount():
+            if sel < 0 or sel >= self.GetCount():
                 break
 
             prop = self._props[sel]
             if prop.IsVisible():
                 self.SetSelection(sel)
                 self.EnsureVisible(sel)
                 break
@@ -463,14 +485,31 @@
         for p in self._props:
             if p.IsVisible():
                 h = p.GetMinSize().y
                 p.SetRect(wx.Rect(0, y, w, h))
                 # let art provider update drawing regions (e.g., value rect)
                 self._art.PrepareDrawRect(p)
                 y += h
+        prev_prop = None
+        for p in self._props:
+            if not  p.IsVisible():
+                continue
+            p.top_value_border = False
+            if prev_prop is None or prev_prop.IsSeparator() or p.IsSeparator():
+                p.top_value_border = True
+            prev_prop = p
+
+        next_prop = None
+        for p in reversed(self._props):
+            if not  p.IsVisible():
+                continue
+            p.bottom_value_border = False
+            if next_prop is None or next_prop.IsSeparator() or p.IsSeparator():
+                p.bottom_value_border = True
+            next_prop = p
 
     def GetDrawRect(self):
         """return the drawing rect"""
         sz = self.GetClientSize()
         rc = wx.Rect(0, 0, sz.x, sz.y)
 
         # shift the client rectangle to take into account scrolling, converting
@@ -479,15 +518,15 @@
 
         return rc
 
     def CheckProp(self):
         """update the property status"""
         parent = None
         for i, prop in enumerate(self._props):
-            parent = self.GetProperty(i - 1)
+            parent = self.Get(i - 1)
             # find the direct parent property
             while parent:
                 if parent.GetIndent() < prop.GetIndent():
                     break
                 parent = parent.GetParent()
             prop.SetParent(parent)
             if parent:
@@ -506,16 +545,16 @@
             else:
                 # prop with parent depends on parent's status
                 show = parent.IsExpanded() and parent.IsVisible()
             prop.SetVisible(show)
 
     def OnPropRefresh(self, evt):
         """refresh the property, for example, due to value changed"""
-        self.SendPropEvent(evt.GetEventType(), evt.GetProperty())
-        prop = evt.GetProperty()
+        self.SendPropEvent(evt.GetEventType(), evt.GetProp())
+        prop = evt.GetProp()
         if prop is None:
             return
         rc = prop.GetRect()
         rc.x, rc.y = self.CalcScrolledPosition(rc.x, rc.y)
         self.RefreshRect(rc, True)
 
     def GetContextMenu(self, prop):
@@ -536,37 +575,40 @@
         menu.Append(self.ID_PROP_GRID_DELETE, "&Delete")
         menu.AppendSeparator()
         menu.Append(self.ID_PROP_GRID_PROP, "&Properties")
         return menu
 
     def OnPropEventsHandler(self, evt):
         """process the property notification"""
-        if not self.SendPropEvent(evt.GetEventType(), evt.GetProperty()):
+        if not self.SendPropEvent(evt.GetEventType(), evt.GetProp()):
             # vetoed by parent, ignore the event
             return False
 
         eid = evt.GetEventType()
         if eid in [
                 wxEVT_PROP_COLLAPSED, wxEVT_PROP_EXPANDED, wxEVT_PROP_INDENT,
                 wxEVT_PROP_RESIZE
         ]:
             self.UpdateGrid()
         elif eid == wxEVT_PROP_RIGHT_CLICK:
-            menu = self.GetContextMenu(evt.GetProperty())
-            cmd = PopupMenu(self, menu)
-            self.OnProcessCommand(cmd, evt.GetProperty())
+            prop = evt.GetProp()
+            if self.IsConfigurable() and prop.IsConfigurable():
+                # show configuration menu
+                menu = self.GetContextMenu(prop)
+                cmd = PopupMenu(self, menu)
+                self.OnProcessCommand(cmd, prop)
         return True
 
     def OnProcessCommand(self, eid, prop):
         """process the context menu command"""
         if not prop:
             return
 
         if eid == self.ID_PROP_GRID_DELETE:
-            self.DeleteProperty(prop)
+            self.Delete(prop)
         elif eid == self.ID_PROP_GRID_READ_ONLY:
             prop.SetReadonly(not prop.IsReadonly())
         elif eid == self.ID_PROP_GRID_PROP:
             dlg = PropSettings(self, prop)
             if dlg.ShowModal() == wx.ID_OK:
                 # Update the prop only may not be enough, for example, if its
                 # indent is changed, it may affect the previous prop.
@@ -576,15 +618,16 @@
         elif eid == self.ID_PROP_GRID_INDENT_DES:
             prop.SetIndent(prop.GetIndent() - 1)
         elif eid == self.ID_PROP_GRID_MOVE_UP:
             self.MoveProperty(prop, -1)
         elif eid == self.ID_PROP_GRID_MOVE_DOWN:
             self.MoveProperty(prop, 2)
         elif eid == self.ID_PROP_GRID_ADD_SEP:
-            self.InsertSeparator(index=self.GetSelection())
+            prop = PropSeparator().Label('Separator')
+            self.Insert(prop)
 
     def OnKeyDown(self, evt):
         """key down event"""
         prop = self.prop_selected
         skip = True
         if prop:
             skip = False
@@ -617,15 +660,15 @@
                     # Ctrl + Down move the property down
                     self.MovePropertyDown(index)
                 else:
                     # Down select the property below
                     self.NavigateProp(True)
             elif keycode == wx.WXK_DELETE:
                 # delete the property
-                self.RemoveProperty(self.GetSelectedProperty())
+                self.Remove(self.GetSelected())
             else:
                 skip = True
         if skip:
             evt.Skip()
 
     def OnPaint(self, event):
         """draw the property"""
@@ -650,14 +693,15 @@
         # draw the properties
         for p in self._props:
             if not p.IsVisible():
                 continue
             rc_prop = p.GetRect()
             if rc.Intersects(rc_prop):
                 self._art.DrawItem(dc, p)
+                p.PostRefresh()
 
     def OnSize(self, evt):
         """resize the properties"""
         self.UpdateGrid()
         evt.Skip()
 
     def OnEraseBackground(self, evt):
@@ -668,114 +712,120 @@
     def OnMouseDown(self, evt):
         """left mouse down"""
         # find the property under mouse
         pt = self.CalcUnscrolledPosition(evt.GetPosition())
         index = self.PropHitTest(pt)
         self.pos_mouse_down = pt
         if index != -1:
-            prop = self.GetProperty(index)
+            prop = self.Get(index)
 
             # pass the event to the property
             ht = prop.OnMouseDown(pt)
             self.prop_under_mouse = prop
-            self.CaptureMouse()
+            self._set_capture(True)
             self.resize_mode = self.RESIZE_NONE
             if ht == 'splitter':
                 # drag the splitter
                 self.resize_mode = self.RESIZE_SEP
             elif ht == 'bottom_edge':
                 # drag the bottom edge
                 self.resize_mode = self.RESIZE_BOT
             elif ht == 'top_edge':
                 # drag the bottom edge of the property above
                 if index > 0:
                     index = index - 1
-                    self.prop_under_mouse = self.GetProperty(index)
+                    self.prop_under_mouse = self.Get(index)
                     self.resize_mode = self.RESIZE_BOT
-            elif ht == 'label':
+            elif ht == 'label' or ht is None:
                 # start drag & drop
-                PropGrid.drag_start = self.ClientToScreen(pt)
-                PropGrid.drag_prop = prop
-                PropGrid.drag_state = 1
+                if self.IsDraggable() and prop.IsDraggable():
+                    PropGrid.drag_start = self.ClientToScreen(pt)
+                    PropGrid.drag_prop = prop
+                    PropGrid.drag_pg = self
+                    PropGrid.drag_state = 1
         # activate the property under mouse
         self.SetSelection(index)
         evt.Skip()
 
     def OnMouseUp(self, evt):
         """left mouse up"""
         if self.prop_under_mouse:
             pt = self.CalcUnscrolledPosition(evt.GetPosition())
             # pass the event to the property
             self.prop_under_mouse.OnMouseUp(pt)
             self.prop_under_mouse = None
 
-        if self.GetCapture() == self:
-            self.ReleaseMouse()
+        self._set_capture(False)
 
         # finish resizing
         self.pos_mouse_down = wx.Point(0, 0)
         self.resize_mode = self.RESIZE_NONE
 
-        # finish drag & drop
-        PropGrid.drag_prop = None
-        PropGrid.drag_state = 0
-        PropGrid.drag_start = wx.Point(0, 0)
-
         evt.Skip()
 
+    def _set_capture(self, capture=True):
+        """Control wx mouse capture."""
+        if self.HasCapture():
+            self.ReleaseMouse()
+        if capture:
+            self.CaptureMouse()
+
     def OnMouseDoubleClick(self, evt):
         """double click"""
         pt = self.CalcUnscrolledPosition(evt.GetPosition())
         index = self.PropHitTest(pt)
         if index != -1:
             # pass the event to the property
-            prop = self.GetProperty(index)
+            prop = self.Get(index)
             prop.OnMouseDoubleClick(pt)
 
         evt.Skip()
 
     def OnMouseCaptureLost(self, evt):
-        pass
+        self._set_capture(False)
 
     def OnMouseMove(self, evt):
         """mouse move"""
         pt = self.CalcUnscrolledPosition(evt.GetPosition())
         index = self.PropHitTest(pt)
         prop = None
         if index != -1:
             # pass the event to the property
-            prop = self.GetProperty(index)
+            prop = self.Get(index)
             prop.OnMouseMove(pt)
+
         # drag & drop
         if evt.LeftIsDown() and PropGrid.drag_prop and\
            PropGrid.drag_state == 1:
             pt = self.ClientToScreen(pt)
             start = PropGrid.drag_start
             if (start.x - pt.x)**2 + (start.y - pt.y)**2 > 10:
                 if self.SendPropEvent(wxEVT_PROP_BEGIN_DRAG, self.drag_prop):
                     # the mouse is moved, so start drag & drop
                     PropGrid.drag_state = 2
-                    PropGrid.drag_pg = self
                     # start drag operation
+                    self._set_capture(False)
                     propData = wx.TextDataObject(PropGrid.drag_prop.GetName())
                     source = wx.DropSource(PropGrid.drag_pg)
                     source.SetData(propData)
-
-                    rtn = source.DoDragDrop(True)
+                    rtn = source.DoDragDrop(wx.Drag_AllowMove)
                     if rtn == wx.DragError:
                         wx.LogError("An error occurred during drag \
                                      and drop operation")
                     elif rtn == wx.DragNone:
                         pass
                     elif rtn == wx.DragCopy:
                         pass
                     elif rtn == wx.DragMove:
                         pass
                     elif rtn == wx.DragCancel:
                         pass
+                    # finish drag & drop
+                    PropGrid.drag_prop = None
+                    PropGrid.drag_start = wx.Point(0, 0)
                     PropGrid.drag_state = 0
                     PropGrid.drag_pg = None
 
         if evt.LeftIsDown() and self.prop_under_mouse:
             # resize the property
             if self.resize_mode == self.RESIZE_SEP:
                 # resize the title width for all properties
@@ -826,14 +876,16 @@
                     self.cursor_mode = mode
                     if mode == self.CURSOR_RESIZE_HORZ:
                         self.SetCursor(self.resize_cursor_horz)
                     elif mode == self.CURSOR_RESIZE_VERT:
                         self.SetCursor(self.resize_cursor_vert)
                     else:
                         self.SetCursor(wx.NullCursor)
+
+
         evt.Skip()
 
     def OnMouseLeave(self, evt):
         """mouse leaves the window"""
         self.SetCursor(wx.NullCursor)
         evt.Skip()
 
@@ -841,171 +893,178 @@
         """right click"""
         pt = self.CalcUnscrolledPosition(evt.GetPosition())
         index = self.PropHitTest(pt)
         # set the active property
         self.SetSelection(index)
         if index != -1:
             # pass the event to the property
-            prop = self.GetProperty(index)
+            prop = self.Get(index)
             prop.OnMouseRightClick(pt)
 
-    def OnDrop(self, x, y, name):
-        """drop the property"""
+    def doDrop(self, x, y, name):
         pt = wx.Point(x, y)
         pt = self.CalcUnscrolledPosition(pt)
         index2 = self.PropHitTest(pt)
-        prop = self.GetProperty(index2)
+        prop = self.Get(index2)
         # insert a property? Let the parent to determine what to do
         if PropGrid.drag_prop is None:
             dp.send('prop.drop', index=index2, prop=name, grid=self)
             return
 
         if name != PropGrid.drag_prop.GetName():
             # something is wrong
             return
 
-        index = PropGrid.drag_pg.FindPropertyIndex(PropGrid.drag_prop)
+        index = PropGrid.drag_pg.Index(PropGrid.drag_prop)
         if index == -1:
             # not find the dragged property, do nothing
             return
 
         if PropGrid.drag_pg != self:
             # drop the property from the other window, copy it
             indent = PropGrid.drag_prop.GetIndent()
-            self.CopyProperty(PropGrid.drag_prop, index2)
+            self.CopyProp(PropGrid.drag_prop, index2)
             for i in six.moves.range(index + 1,
-                                     PropGrid.drag_pg.GetPropCount()):
+                                     PropGrid.drag_pg.GetCount()):
                 # copy all its children
-                child = PropGrid.drag_pg.GetProperty(i)
+                child = PropGrid.drag_pg.Get(i)
                 if child.GetIndent() <= indent:
                     break
                 if index2 != -1:
                     index2 = index2 + 1
-                self.CopyProperty(child, index2)
+                self.CopyProp(child, index2)
         else:
             # move the property if necessary
             if prop == PropGrid.drag_prop:
                 return
             self.doMoveProperty(index, index2)
         self.UpdateGrid()
 
+    def OnDrop(self, x, y, name):
+        """drop the property"""
+        self.OnLeave()
+        self.doDrop(x, y, name)
+
+    def OnDragOver(self, x, y, d):
+        pt = wx.Point(x, y)
+        rc = self.GetClientRect()
+        if rc.Contains(pt):
+            (x, y) = self.GetViewStart()
+            if pt.y < 15:
+                self.Scroll(-1, y - (15 - pt.y) / 3)
+            if pt.y > rc.bottom - 15:
+                self.Scroll(-1, y - (rc.bottom - 15 - pt.y) / 3)
+
+        if self.drag_image:
+            self.drag_image.Hide()
+        if PropGrid.drag_prop and PropGrid.drag_pg == self:
+            # only do drop if we are moving the prop in the same propgrid;
+            # it is more complicated if moved from another propgrid (e.g.,
+            # first moved in, insert prop, then move; if mouse moves away, delete)
+            self.doDrop(pt.x, pt.y, PropGrid.drag_prop.GetName())
+        if self.drag_image:
+            self.drag_image.Move(pt)
+            self.drag_image.Show()
+
+    def OnEnter(self, x, y, d):
+        if self.HasCapture():
+            self.ReleaseMouse()
+        self.OnLeave()
+        if PropGrid.drag_prop:
+            if wx.Platform == "__WXMAC__":
+                # not work on GTK3
+                self.drag_bitmap = self.CreateDragImage(PropGrid.drag_prop)
+                self.drag_image = wx.DragImage(self.drag_bitmap)
+                self.drag_image.BeginDrag(wx.Point(0,0), self)
+                self.drag_image.Move(wx.Point(x, y))
+                self.drag_image.Show()
+
+    def OnLeave(self):
+        if self.drag_image:
+            self.drag_image.Hide()
+            self.drag_image.EndDrag()
+            self.drag_image = None
 
 class PropSettings(wx.Dialog):
     def __init__(self, parent, prop):
         wx.Dialog.__init__(self,
                            parent,
                            title="Settings...",
                            size=wx.Size(600, 460),
                            style=wx.DEFAULT_DIALOG_STYLE | wx.RESIZE_BORDER)
 
-        self.propgrid = PropGrid(self)
+        self.propgrid = PropGrid(self).Configurable(False)
         self.propgrid.GetArtProvider().SetTitleWidth(200)
         self.prop = prop
         if prop.IsSeparator():
-            self.items = (('name', 'Name', '', 'editbox'), ('label', 'Label',
-                                                            '', 'editbox'),
-                          ('indent', 'Indent level', '', 'spin'),
-                          ('font_label', 'Label font', '_font_label', 'font'),
-                          ('font_value', 'Value font', '_font_value', 'font'))
+            self.items = (('name', PropText().Label('Name'), ''),
+                          ('label', PropText().Label('Label'), ''),
+                          ('indent',PropSpin(0, 100).Label('Indent level'), ''),
+                          ('font_label', PropFont().Label('Label font'), '_font_label'),
+                          ('font_value', PropFont().Label('Value font'), '_font_value'))
         else:
-            self.items = (('name', 'Name', '', 'editbox'), ('label', 'Label',
-                                                            '', 'editbox'),
-                          ('indent', 'Indent level', '',
-                           'spin'), ('enable', 'Enable', '', 'checkbox'),
-                          ('font_label', 'Label font', '_font_label',
-                           'font'), ('font_value', 'Value font', '_font_value',
-                                     'font'), ('readonly', 'Read only', '',
-                                               'checkbox'),
-                          ('text_clr', 'Normal text color', 'text_clr',
-                           'color'), ('text_clr_sel', 'Selected text color',
-                                      'text_clr_sel', 'color'),
-                          ('text_clr_disabled', 'Disable text color',
-                           'text_clr_disabled', 'color'),
-                          ('bg_clr', 'Normal background color', 'bg_clr',
-                           'color'), ('bg_clr_sel',
-                                      'Selected background color',
-                                      'bg_clr_sel', 'color'),
-                          ('bg_clr_disabled', 'Disabled background color',
-                           'bg_clr_disabled', 'color'))
+            self.items = (('name', PropText('Name'), ''),
+                          ('label', PropText('Label'), ''),
+                          ('indent', PropSpin(0, 100, 'Indent level'), ''),
+                          ('enable', PropCheckBox('Enable'), ''),
+                          ('font_label', PropFont('Label font'), '_font_label'),
+                          ('font_value', PropFont('Value font'), '_font_value'),
+                          ('readonly', PropCheckBox('Read only'), ''),
+                          ('text_clr', PropColor('Normal text color'), 'text_clr'),
+                          ('text_clr_sel', PropColor('Selected text color'), 'text_clr_sel'),
+                          ('text_clr_disabled', PropColor('Disable text color'), 'text_clr_disabled'),
+                          ('bg_clr', PropColor('Normal background color'), 'bg_clr'),
+                          ('bg_clr_sel', PropColor('Selected background color'), 'bg_clr_sel'),
+                          ('bg_clr_disabled', PropColor('Disabled background color'), 'bg_clr_disabled'))
 
-        for (name, label, gname, ctrl) in self.items:
-            pp = self.propgrid.InsertProperty(name, label, '')
+        for (name, pp, gname) in self.items:
+            pp = self.propgrid.Insert(pp.Name(name))
             if prop:
                 v = getattr(prop, name)
             else:
                 v = ""
             if v is None and gname:
                 v = getattr(prop.grid.GetArtProvider(), gname)
 
-            pp.SetLabelTip(label)
-            pp.SetControlStyle(ctrl)
-            if ctrl == 'checkbox':
-                pp.SetValue(v)
-                pp.SetFormatter(BoolFormatter())
-            elif ctrl == 'color':
-                pp.SetValue(v)
-                pp.SetBgColor(v, v, v)
-                t = wx.Colour(v)
-                t.SetRGB(t.GetRGB() ^ 0xffffff)
-                t = t.GetAsString(wx.C2S_HTML_SYNTAX)
-                pp.SetTextColor(t, t, t)
-                pp.SetFormatter(ColorFormatter())
-            elif ctrl == 'font':
-                pp.SetValueFont(v)
-                pp.SetValue(v)
-                pp.SetFormatter(FontFormatter())
-            elif ctrl in ['spin', 'slider']:
-                pp.SetFormatter(IntFormatter(0, 100))
-                pp.SetValue(v)
-            else:
-                pp.SetValue(v)
+            pp.SetValue(v)
 
         sz = wx.BoxSizer(wx.VERTICAL)
         sz.Add(self.propgrid, 1, wx.EXPAND | wx.ALL, 1)
 
         self.stcline = wx.StaticLine(self, style=wx.LI_HORIZONTAL)
         sz.Add(self.stcline, 0, wx.EXPAND | wx.ALL, 5)
 
-        sz2 = wx.BoxSizer(wx.HORIZONTAL)
-        sz2.Add(wx.Button(self, wx.ID_OK, u"&Ok"), 0, wx.ALL, 5)
-        sz2.Add(wx.Button(self, wx.ID_CANCEL, u"&Cancel"), 0, wx.ALL, 5)
-        sz.Add(sz2, 0, wx.ALIGN_RIGHT | wx.RIGHT, 5)
+
+        btnsizer = wx.StdDialogButtonSizer()
+        btnsizer.AddStretchSpacer(1)
+
+        btn = wx.Button(self, wx.ID_OK)
+        btn.SetDefault()
+        btnsizer.AddButton(btn)
+
+        btn = wx.Button(self, wx.ID_CANCEL)
+        btnsizer.AddButton(btn)
+        btnsizer.Realize()
+
+        sz.Add(btnsizer, 0, wx.ALIGN_RIGHT | wx.RIGHT, 5)
 
         self.SetSizer(sz)
         self.Layout()
 
         # Connect Events
         self.Bind(wx.EVT_BUTTON, self.OnBtnOk, id=wx.ID_OK)
-        self.Bind(EVT_PROP_RIGHT_CLICK, self.OnPropEventsHandler)
-        self.Bind(EVT_PROP_CHANGED, self.OnPropChanged)
-
-    def OnPropEventsHandler(self, evt):
-        # disable context menu
-        evt.Veto()
-
-    def OnPropChanged(self, evt):
-        p = evt.GetProperty()
-        if '_clr' in p.GetName():
-            t = wx.Colour(p.GetValue())
-            c = t.GetAsString(wx.C2S_HTML_SYNTAX)
-            p.SetBgColor(c, c, c)
-            t.SetRGB(t.GetRGB() ^ 0xFFFFFF)
-            t = t.GetAsString(wx.C2S_HTML_SYNTAX)
-            p.SetTextColor(t, t, t)
-        elif 'font_' in p.GetName():
-            p.SetValueFont(p.GetValue())
 
     def OnBtnOk(self, event):
         if self.propgrid.prop_selected:
             # update the value if necessary
             self.propgrid.prop_selected.OnTextEnter()
 
-        for (name, _, _, ctrl) in self.items:
-            v = self.propgrid.GetProperty(name)
-            if ctrl == 'checkbox':
+        for (name, pp, _ ) in self.items:
+            v = self.propgrid.Get(name)
+            if isinstance(pp, PropCheckBox):
                 setattr(self.prop, name, bool(int(v.GetValue())))
             if getattr(self.prop, name) is None:
                 setattr(self.prop, name, v.GetValue())
             else:
                 setattr(self.prop, name,
                         type(getattr(self.prop, name))(v.GetValue()))
         event.Skip()
```

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/propxpm.py` & `bsmedit-3.2.9/bsmedit/propgrid/propxpm.py`

 * *Files identical despite different names*

### Comparing `bsmedit-3.2.8/bsmedit/propgrid/validators.py` & `bsmedit-3.2.9/bsmedit/propgrid/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,17 @@
         Only copies data if value is actually changed from attribute value.
         """
         try:
             if self.obj is None:
                 # Nothing to do
                 return True
 
+            if not self.Validate(self.GetWindow()):
+                return False
+
             # Get widget value
             val = self._getControlValue()
 
             # Check widget value against attribute value; only copy if changed
             # Get object attribute value
             old_val = getattr(self.obj, self.attr)
             if self.formatter:
```


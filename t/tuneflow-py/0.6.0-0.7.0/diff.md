# Comparing `tmp/tuneflow-py-0.6.0.tar.gz` & `tmp/tuneflow-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.6.0.tar", last modified: Sun Apr 16 21:26:52 2023, max compression
+gzip compressed data, was "tuneflow-py-0.7.0.tar", last modified: Sat Apr 29 04:12:50 2023, max compression
```

## Comparing `tuneflow-py-0.6.0.tar` & `tuneflow-py-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.6.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.6.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-16 21:26:20.000000 tuneflow-py-0.6.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.6.0/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.6.0/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.6.0/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    71614 2023-04-15 03:58:44.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25607 2023-04-10 18:24:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.6.0/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.6.0/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.722991 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-16 21:26:52.000000 tuneflow-py-0.6.0/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-16 21:26:52.732991 tuneflow-py-0.6.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.6.0/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.6.0/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.6.0/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.6.0/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.6.0/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.6.0/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.6.0/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.6.0/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.7.0/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.7.0/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-29 04:12:20.000000 tuneflow-py-0.7.0/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.7.0/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.7.0/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.7.0/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.7.0/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/test/test_lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.7.0/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.7.0/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.7.0/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.7.0/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.7.0/test/test_utils.py
```

### Comparing `tuneflow-py-0.6.0/LICENSE` & `tuneflow-py-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/PKG-INFO` & `tuneflow-py-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.6.0
+Version: 0.7.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.6.0/README.md` & `tuneflow-py-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/pyproject.toml` & `tuneflow-py-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.6.0"
+version = "0.7.0"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/__init__.py` & `tuneflow-py-0.7.0/src/tuneflow_py/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from tuneflow_py.base_plugin import TuneflowPlugin
 from tuneflow_py.models.audio_plugin import AudioPlugin, get_audio_plugin_tuneflow_id, are_tuneflow_ids_equal, are_tuneflow_ids_equal_ignore_version, decode_audio_plugin_tuneflow_id
 from tuneflow_py.models.automation import AutomationTarget, AutomationTargetType, AutomationData, AutomationPoint, AutomationValue
 from tuneflow_py.models.clip import ClipType, Clip
 from tuneflow_py.models.note import Note
 from tuneflow_py.models.song import Song
+from tuneflow_py.models.lyric import Lyrics, LyricLine, LyricWord
 from tuneflow_py.models.tempo import TempoEvent
 from tuneflow_py.models.marker import StructureMarker, StructureType
 from tuneflow_py.models.time_signature import TimeSignatureEvent
 from tuneflow_py.models.track import TrackType, Track, TrackOutputType
 from tuneflow_py.descriptors.widget import *
 from tuneflow_py.descriptors.text import *
 from tuneflow_py.descriptors.param import *
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.7.0/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/note.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='song.proto',
   package='song',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\x9e\x01\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\x12\x13\n\x0bspeed_ratio\x18\x05 \x01(\x01\x12\x14\n\x0cpitch_offset\x18\x06 \x01(\x01\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xf6\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\x12\x13\n\x0b\x63ustom_name\x18\x03 \x01(\t\"\x8c\x01\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\x12\x0e\n\nPRE_CHORUS\x10\x06\x12\x0f\n\x0bPOST_CHORUS\x10\x07\x12\x08\n\x04\x46ILL\x10\x08\x12\n\n\x06\x43USTOM\x10\t\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x92\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
+  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\x9e\x01\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\x12\x13\n\x0bspeed_ratio\x18\x05 \x01(\x01\x12\x14\n\x0cpitch_offset\x18\x06 \x01(\x01\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xf6\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\x12\x13\n\x0b\x63ustom_name\x18\x03 \x01(\t\"\x8c\x01\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\x12\x0e\n\nPRE_CHORUS\x10\x06\x12\x0f\n\x0bPOST_CHORUS\x10\x07\x12\x08\n\x04\x46ILL\x10\x08\x12\n\n\x06\x43USTOM\x10\t\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xb0\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus\x12\x1c\n\x06lyrics\x18\n \x01(\x0b\x32\x0c.song.Lyrics\"(\n\x06Lyrics\x12\x1e\n\x05lines\x18\x01 \x03(\x0b\x32\x0f.song.LyricLine\"v\n\tLyricLine\x12(\n\x05words\x18\x01 \x03(\x0b\x32\x19.song.LyricLine.LyricWord\x1a?\n\tLyricWord\x12\x12\n\nstart_tick\x18\x01 \x01(\x05\x12\x10\n\x08\x65nd_tick\x18\x02 \x01(\x05\x12\x0c\n\x04word\x18\x03 \x01(\t*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
 )
 
 _TRACKTYPE = _descriptor.EnumDescriptor(
   name='TrackType',
   full_name='song.TrackType',
   filename=None,
   file=DESCRIPTOR,
@@ -54,16 +54,16 @@
       name='AUX_TRACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3140,
-  serialized_end=3238,
+  serialized_start=3332,
+  serialized_end=3430,
 )
 _sym_db.RegisterEnumDescriptor(_TRACKTYPE)
 
 TrackType = enum_type_wrapper.EnumTypeWrapper(_TRACKTYPE)
 _CLIPTYPE = _descriptor.EnumDescriptor(
   name='ClipType',
   full_name='song.ClipType',
@@ -85,16 +85,16 @@
       name='AUDIO_CLIP', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3240,
-  serialized_end=3301,
+  serialized_start=3432,
+  serialized_end=3493,
 )
 _sym_db.RegisterEnumDescriptor(_CLIPTYPE)
 
 ClipType = enum_type_wrapper.EnumTypeWrapper(_CLIPTYPE)
 UNDEFINED_TRACK = 0
 MIDI_TRACK = 1
 AUDIO_TRACK = 2
@@ -1439,28 +1439,144 @@
     _descriptor.FieldDescriptor(
       name='buses', full_name='song.Song.buses', index=8,
       number=9, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='lyrics', full_name='song.Song.lyrics', index=9,
+      number=10, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=2864,
-  serialized_end=3138,
+  serialized_end=3168,
+)
+
+
+_LYRICS = _descriptor.Descriptor(
+  name='Lyrics',
+  full_name='song.Lyrics',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='lines', full_name='song.Lyrics.lines', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3170,
+  serialized_end=3210,
+)
+
+
+_LYRICLINE_LYRICWORD = _descriptor.Descriptor(
+  name='LyricWord',
+  full_name='song.LyricLine.LyricWord',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='start_tick', full_name='song.LyricLine.LyricWord.start_tick', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='end_tick', full_name='song.LyricLine.LyricWord.end_tick', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='word', full_name='song.LyricLine.LyricWord.word', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3267,
+  serialized_end=3330,
+)
+
+_LYRICLINE = _descriptor.Descriptor(
+  name='LyricLine',
+  full_name='song.LyricLine',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='words', full_name='song.LyricLine.words', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_LYRICLINE_LYRICWORD, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3212,
+  serialized_end=3330,
 )
 
 _AUTOMATIONTARGET.fields_by_name['type'].enum_type = _AUTOMATIONTARGET_TARGETTYPE
 _AUTOMATIONTARGET_TARGETTYPE.containing_type = _AUTOMATIONTARGET
 _AUTOMATIONVALUE_PARAMVALUE.containing_type = _AUTOMATIONVALUE
 _AUTOMATIONVALUE.fields_by_name['points'].message_type = _AUTOMATIONVALUE_PARAMVALUE
 _AUTOMATIONDATA_TARGETVALUESENTRY.fields_by_name['value'].message_type = _AUTOMATIONVALUE
@@ -1494,14 +1610,18 @@
 _STRUCTUREMARKER_STRUCTURETYPE.containing_type = _STRUCTUREMARKER
 _SONG.fields_by_name['tempos'].message_type = _TEMPOEVENT
 _SONG.fields_by_name['time_signatures'].message_type = _TIMESIGNATUREEVENT
 _SONG.fields_by_name['tracks'].message_type = _TRACK
 _SONG.fields_by_name['master_track'].message_type = _TRACK
 _SONG.fields_by_name['structures'].message_type = _STRUCTUREMARKER
 _SONG.fields_by_name['buses'].message_type = _BUS
+_SONG.fields_by_name['lyrics'].message_type = _LYRICS
+_LYRICS.fields_by_name['lines'].message_type = _LYRICLINE
+_LYRICLINE_LYRICWORD.containing_type = _LYRICLINE
+_LYRICLINE.fields_by_name['words'].message_type = _LYRICLINE_LYRICWORD
 DESCRIPTOR.message_types_by_name['Note'] = _NOTE
 DESCRIPTOR.message_types_by_name['TempoEvent'] = _TEMPOEVENT
 DESCRIPTOR.message_types_by_name['TimeSignatureEvent'] = _TIMESIGNATUREEVENT
 DESCRIPTOR.message_types_by_name['InstrumentInfo'] = _INSTRUMENTINFO
 DESCRIPTOR.message_types_by_name['AudioPluginInfo'] = _AUDIOPLUGININFO
 DESCRIPTOR.message_types_by_name['AutomationTarget'] = _AUTOMATIONTARGET
 DESCRIPTOR.message_types_by_name['AutomationValue'] = _AUTOMATIONVALUE
@@ -1512,14 +1632,16 @@
 DESCRIPTOR.message_types_by_name['Track'] = _TRACK
 DESCRIPTOR.message_types_by_name['AudioData'] = _AUDIODATA
 DESCRIPTOR.message_types_by_name['AudioClipData'] = _AUDIOCLIPDATA
 DESCRIPTOR.message_types_by_name['Clip'] = _CLIP
 DESCRIPTOR.message_types_by_name['StructureMarker'] = _STRUCTUREMARKER
 DESCRIPTOR.message_types_by_name['Bus'] = _BUS
 DESCRIPTOR.message_types_by_name['Song'] = _SONG
+DESCRIPTOR.message_types_by_name['Lyrics'] = _LYRICS
+DESCRIPTOR.message_types_by_name['LyricLine'] = _LYRICLINE
 DESCRIPTOR.enum_types_by_name['TrackType'] = _TRACKTYPE
 DESCRIPTOR.enum_types_by_name['ClipType'] = _CLIPTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Note = _reflection.GeneratedProtocolMessageType('Note', (_message.Message,), {
   'DESCRIPTOR' : _NOTE,
   '__module__' : 'song_pb2'
@@ -1674,13 +1796,35 @@
 Song = _reflection.GeneratedProtocolMessageType('Song', (_message.Message,), {
   'DESCRIPTOR' : _SONG,
   '__module__' : 'song_pb2'
   # @@protoc_insertion_point(class_scope:song.Song)
   })
 _sym_db.RegisterMessage(Song)
 
+Lyrics = _reflection.GeneratedProtocolMessageType('Lyrics', (_message.Message,), {
+  'DESCRIPTOR' : _LYRICS,
+  '__module__' : 'song_pb2'
+  # @@protoc_insertion_point(class_scope:song.Lyrics)
+  })
+_sym_db.RegisterMessage(Lyrics)
+
+LyricLine = _reflection.GeneratedProtocolMessageType('LyricLine', (_message.Message,), {
+
+  'LyricWord' : _reflection.GeneratedProtocolMessageType('LyricWord', (_message.Message,), {
+    'DESCRIPTOR' : _LYRICLINE_LYRICWORD,
+    '__module__' : 'song_pb2'
+    # @@protoc_insertion_point(class_scope:song.LyricLine.LyricWord)
+    })
+  ,
+  'DESCRIPTOR' : _LYRICLINE,
+  '__module__' : 'song_pb2'
+  # @@protoc_insertion_point(class_scope:song.LyricLine)
+  })
+_sym_db.RegisterMessage(LyricLine)
+_sym_db.RegisterMessage(LyricLine.LyricWord)
+
 
 _AUTOMATIONDATA_TARGETVALUESENTRY._options = None
 _TRACK_AUDIOPLUGINENTRY._options = None
 _TRACK_SENDSENTRY._options = None
 _TRACK.fields_by_name['notes']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/song.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/song.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         # Delete dependencies.
         for dep_track in self.get_tracks():
             track_output = dep_track.get_output()
             if track_output is not None and track_output.get_type() == TrackOutputType.TRACK_OUTPUT_TRACK and track_output.get_track_id() == track_id:
                 dep_track.remove_output()
         return track
 
+    def get_lyrics(self):
+        return self._proto.lyrics
+
     def get_structures(self):
         return [StructureMarker(song=self, proto=structure_proto) for structure_proto in self._proto.structures]
 
     def get_structure_at_index(self, index: int):
         if index < 0 or index >= len(self._proto.structures):
             return None
         return StructureMarker(song=self, proto=self._proto.structures[index])
@@ -128,15 +131,15 @@
 
     def move_structure(self, structure_index: int, move_to_tick: int):
         structure = self.get_structure_at_index(structure_index)
         if not structure:
             return
         if structure_index <= 0:
             return
-        prev_structure : StructureMarker = self.get_structure_at_index(structure_index - 1)
+        prev_structure: StructureMarker = self.get_structure_at_index(structure_index - 1)
         if prev_structure.get_tick() == move_to_tick:
             # Moved to another structure, delete it.
             self.remove_structure(structure_index - 1)
         elif structure_index < len(self.get_structures()) - 1:
             next_structure = self.get_structure_at_index(structure_index + 1)
             if next_structure and next_structure.get_tick() == move_to_tick:
                 # Moved to another time signature, delete it.
@@ -195,15 +198,15 @@
 
         def scale_int_by(value, scale_factor):
             return round(value * scale_factor)
 
         song = Song()
         song_proto = song._proto
         ppq_scale_factor = float(song_proto.PPQ) / \
-                           float(midi_obj.ticks_per_beat)
+            float(midi_obj.ticks_per_beat)
         # Add tempos and time signatures
         song.overwrite_tempo_changes([TempoEvent(ticks=scale_int_by(
             tempo_change.time, ppq_scale_factor), bpm=tempo_change.tempo) for tempo_change in midi_obj.tempo_changes])
         song.overwrite_time_signature_changes([
             TimeSignatureEvent(
                 ticks=scale_int_by(time_signature_change.time, ppq_scale_factor),
                 numerator=time_signature_change.numerator,
@@ -592,7 +595,8 @@
 
     @staticmethod
     def get_default_resolution():
         '''
         Returns the default Pulse-per-Quater-Note used in TuneFlow.
         '''
         return 480
+
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/models/track.py` & `tuneflow-py-0.7.0/src/tuneflow_py/models/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from tuneflow_py.descriptors.clip_descriptor import AudioClipData
 from tuneflow_py.models.protos import song_pb2
 from tuneflow_py.models.clip import Clip, ClipType
+from tuneflow_py.models.note import Note
 from tuneflow_py.models.audio_plugin import AudioPlugin
 from tuneflow_py.models.automation import AutomationData
 from tuneflow_py.utils import db_to_volume_value, volume_value_to_db, lower_equal, greater_equal, lower_than, decode_audio_plugin_tuneflow_id
 import nanoid
 from typing import List
 from types import SimpleNamespace
 
@@ -453,7 +454,14 @@
 
     def __repr__(self) -> str:
         return str(self._proto)
 
     @staticmethod
     def _generate_track_id():
         return nanoid.generate()
+
+    def get_visible_notes(self) -> List[Note]:
+        visible_notes = []
+        for clip in self.get_clips():
+            for note in clip.get_notes():
+                visible_notes.append(note)
+        return sorted(visible_notes, key=lambda note: note.get_start_tick())
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py/utils.py` & `tuneflow-py-0.7.0/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.7.0/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.6.0
+Version: 0.7.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.6.0/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.7.0/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 src/tuneflow_py/descriptors/param.py
 src/tuneflow_py/descriptors/plugin.py
 src/tuneflow_py/descriptors/text.py
 src/tuneflow_py/descriptors/widget.py
 src/tuneflow_py/models/audio_plugin.py
 src/tuneflow_py/models/automation.py
 src/tuneflow_py/models/clip.py
+src/tuneflow_py/models/lyric.py
 src/tuneflow_py/models/marker.py
 src/tuneflow_py/models/note.py
 src/tuneflow_py/models/song.py
 src/tuneflow_py/models/tempo.py
 src/tuneflow_py/models/time_signature.py
 src/tuneflow_py/models/track.py
 src/tuneflow_py/models/protos/song_pb2.py
 test/test_audio_clip.py
 test/test_automation.py
+test/test_lyric.py
 test/test_marker.py
 test/test_midi_clip.py
 test/test_note.py
 test/test_song.py
 test/test_track.py
 test/test_utils.py
```

### Comparing `tuneflow-py-0.6.0/test/test_audio_clip.py` & `tuneflow-py-0.7.0/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_automation.py` & `tuneflow-py-0.7.0/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_marker.py` & `tuneflow-py-0.7.0/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_midi_clip.py` & `tuneflow-py-0.7.0/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_note.py` & `tuneflow-py-0.7.0/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_song.py` & `tuneflow-py-0.7.0/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.6.0/test/test_utils.py` & `tuneflow-py-0.7.0/test/test_utils.py`

 * *Files identical despite different names*


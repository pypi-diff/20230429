# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.0a1.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.0a1.tar", last modified: Sat Apr 29 17:05:33 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.0a2.tar", last modified: Sat Apr 29 17:06:43 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1.tar` & `ovos-stt-plugin-fasterwhisper-0.0.0a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:05:33.814801 ovos-stt-plugin-fasterwhisper-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-04-29 17:05:26.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 17:05:26.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:05:33.814801 ovos-stt-plugin-fasterwhisper-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-29 17:05:26.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:05:33.814801 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 17:05:26.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 17:05:29.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:05:33.814801 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:05:33.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:05:33.814801 ovos-stt-plugin-fasterwhisper-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3479 2023-04-29 17:05:26.000000 ovos-stt-plugin-fasterwhisper-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 17:06:39.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3479 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a1/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.py`

 * *Files identical despite different names*


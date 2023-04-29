# Comparing `tmp/openai_rev-1.1.tar.gz` & `tmp/openai_rev-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_rev-1.1.tar", last modified: Sat Apr 29 02:40:23 2023, max compression
+gzip compressed data, was "openai_rev-1.2.tar", last modified: Sat Apr 29 02:44:05 2023, max compression
```

## Comparing `openai_rev-1.1.tar` & `openai_rev-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.764499 openai_rev-1.1/
--rw-------   0 runner    (1000) runner    (1000)     1208 2023-04-29 02:35:21.000000 openai_rev-1.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:40:23.764499 openai_rev-1.1/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      254 2023-04-29 02:35:21.000000 openai_rev-1.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.760499 openai_rev-1.1/openai_rev/
--rw-------   0 runner    (1000) runner    (1000)     2613 2023-04-29 02:39:05.000000 openai_rev-1.1/openai_rev/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-04-29 02:40:09.000000 openai_rev-1.1/openai_rev/__version__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.764499 openai_rev-1.1/openai_rev.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      244 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-29 02:40:23.764499 openai_rev-1.1/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      796 2023-04-29 02:39:22.000000 openai_rev-1.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:44:05.204101 openai_rev-1.2/
+-rw-------   0 runner    (1000) runner    (1000)     1208 2023-04-29 02:35:21.000000 openai_rev-1.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:44:05.204101 openai_rev-1.2/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      254 2023-04-29 02:35:21.000000 openai_rev-1.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:44:05.200101 openai_rev-1.2/openai_rev/
+-rw-------   0 runner    (1000) runner    (1000)     2618 2023-04-29 02:43:56.000000 openai_rev-1.2/openai_rev/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-04-29 02:43:57.000000 openai_rev-1.2/openai_rev/__version__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:44:05.204101 openai_rev-1.2/openai_rev.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:44:05.000000 openai_rev-1.2/openai_rev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      244 2023-04-29 02:44:05.000000 openai_rev-1.2/openai_rev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-29 02:44:05.000000 openai_rev-1.2/openai_rev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-29 02:44:05.000000 openai_rev-1.2/openai_rev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-29 02:44:05.000000 openai_rev-1.2/openai_rev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-29 02:44:05.244101 openai_rev-1.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      796 2023-04-29 02:43:56.000000 openai_rev-1.2/setup.py
```

### Comparing `openai_rev-1.1/LICENSE` & `openai_rev-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_rev-1.1/PKG-INFO` & `openai_rev-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_rev
-Version: 1.1
+Version: 1.2
 Summary: making music with OpenAI (GPT-4)
 Author: bobbill
 License: Unlicense
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `openai_rev-1.1/openai_rev/__init__.py` & `openai_rev-1.2/openai_rev/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
       drum_pattern.append([bass_drum_freq])
     else:
       drum_pattern.append(drum_silence)
 
   return drum_pattern
 
 
-def random(length=120):
+def random_song(length=120):
   c_major_pentatonic = [261.63, 293.66, 329.63, 392.00,
                         440.00]  # C4, D4, E4, G4, A4
   g_major_pentatonic = [392.00, 440.00, 493.88, 587.33,
                         659.25]  # G4, A4, B4, D5, E5
   e_minor_pentatonic = [329.63, 392.00, 440.00, 493.88,
                         587.33]  # E4, G4, A4, B4, D5
```

### Comparing `openai_rev-1.1/openai_rev.egg-info/PKG-INFO` & `openai_rev-1.2/openai_rev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-rev
-Version: 1.1
+Version: 1.2
 Summary: making music with OpenAI (GPT-4)
 Author: bobbill
 License: Unlicense
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `openai_rev-1.1/setup.py` & `openai_rev-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', encoding='utf-8') as f:
   description = f.read()
 
 setuptools.setup(
   name='openai_rev',
-  version='1.1',
+  version='1.2',
   license='Unlicense',
   author='bobbill',
   description='making music with OpenAI (GPT-4)',
   packages=['openai_rev'],
   install_requires=['simpleaudio', 'numpy'],
   long_description=description,
   long_description_content_type='text/markdown',
```


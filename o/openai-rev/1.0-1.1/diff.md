# Comparing `tmp/openai_rev-1.0.tar.gz` & `tmp/openai_rev-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_rev-1.0.tar", last modified: Sat Apr 29 02:36:05 2023, max compression
+gzip compressed data, was "openai_rev-1.1.tar", last modified: Sat Apr 29 02:40:23 2023, max compression
```

## Comparing `openai_rev-1.0.tar` & `openai_rev-1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:36:05.116963 openai_rev-1.0/
--rw-------   0 runner    (1000) runner    (1000)     1208 2023-04-29 02:35:21.000000 openai_rev-1.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:36:05.116963 openai_rev-1.0/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      254 2023-04-29 02:35:21.000000 openai_rev-1.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:36:05.112964 openai_rev-1.0/openai_rev/
--rw-------   0 runner    (1000) runner    (1000)     2675 2023-04-29 02:35:35.000000 openai_rev-1.0/openai_rev/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:36:05.116963 openai_rev-1.0/openai_rev.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:36:03.000000 openai_rev-1.0/openai_rev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      218 2023-04-29 02:36:03.000000 openai_rev-1.0/openai_rev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-29 02:36:03.000000 openai_rev-1.0/openai_rev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-29 02:36:03.000000 openai_rev-1.0/openai_rev.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-29 02:36:03.000000 openai_rev-1.0/openai_rev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-29 02:36:05.116963 openai_rev-1.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      854 2023-04-29 02:35:21.000000 openai_rev-1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.764499 openai_rev-1.1/
+-rw-------   0 runner    (1000) runner    (1000)     1208 2023-04-29 02:35:21.000000 openai_rev-1.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:40:23.764499 openai_rev-1.1/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      254 2023-04-29 02:35:21.000000 openai_rev-1.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.760499 openai_rev-1.1/openai_rev/
+-rw-------   0 runner    (1000) runner    (1000)     2613 2023-04-29 02:39:05.000000 openai_rev-1.1/openai_rev/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-04-29 02:40:09.000000 openai_rev-1.1/openai_rev/__version__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-29 02:40:23.764499 openai_rev-1.1/openai_rev.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      867 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      244 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-29 02:40:23.000000 openai_rev-1.1/openai_rev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-29 02:40:23.764499 openai_rev-1.1/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      796 2023-04-29 02:39:22.000000 openai_rev-1.1/setup.py
```

### Comparing `openai_rev-1.0/LICENSE` & `openai_rev-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_rev-1.0/PKG-INFO` & `openai_rev-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_rev
-Version: 1.0
+Version: 1.1
 Summary: making music with OpenAI (GPT-4)
 Author: bobbill
 License: Unlicense
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `openai_rev-1.0/openai_rev/__init__.py` & `openai_rev-1.1/openai_rev/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 import simpleaudio as sa
 import random
 import numpy as np
 
+
 def play_notes(frequencies, duration):
-    sample_rate = 44100
-    audio_data = np.zeros(int(sample_rate * duration))
-    
-    for frequency in frequencies:
-        t = np.linspace(0, duration, int(sample_rate * duration), False)
-        note_data = np.sin(frequency * t * 2 * np.pi)
-        audio_data += note_data
-    
-    audio_data = (audio_data * 32767 / np.max(np.abs(audio_data))).astype(np.int16)
-    
-    play_obj = sa.play_buffer(audio_data, 1, 2, sample_rate)
-    play_obj.wait_done()
+  sample_rate = 44100
+  audio_data = np.zeros(int(sample_rate * duration))
+
+  for frequency in frequencies:
+    t = np.linspace(0, duration, int(sample_rate * duration), False)
+    note_data = np.sin(frequency * t * 2 * np.pi)
+    audio_data += note_data
+
+  audio_data = (audio_data * 32767 / np.max(np.abs(audio_data))).astype(
+    np.int16)
+
+  play_obj = sa.play_buffer(audio_data, 1, 2, sample_rate)
+  play_obj.wait_done()
+
 
 def generate_chord_progression(progression, key_freqs):
-    chords = []
+  chords = []
+
+  for chord_name in progression:
+    if chord_name == "I":
+      chord_freqs = [key_freqs[0], key_freqs[2], key_freqs[4]]
+    elif chord_name == "IV":
+      chord_freqs = [key_freqs[3], key_freqs[5], key_freqs[0] * 2]
+    elif chord_name == "V":
+      chord_freqs = [key_freqs[4], key_freqs[6], key_freqs[1] * 2]
+    else:
+      raise ValueError("Invalid chord progression symbol")
 
-    for chord_name in progression:
-        if chord_name == "I":
-            chord_freqs = [key_freqs[0], key_freqs[2], key_freqs[4]]
-        elif chord_name == "IV":
-            chord_freqs = [key_freqs[3], key_freqs[5], key_freqs[0] * 2]
-        elif chord_name == "V":
-            chord_freqs = [key_freqs[4], key_freqs[6], key_freqs[1] * 2]
-        else:
-            raise ValueError("Invalid chord progression symbol")
+    chords.append(chord_freqs)
 
-        chords.append(chord_freqs)
+  return chords
 
-    return chords
 
 def generate_melody(frequencies, length):
-    melody = []
+  melody = []
+
+  for _ in range(length):
+    freq = random.choice(frequencies)
+    duration = random.choice([0.125, 0.25,
+                              0.5])  # Add more duration options for variation
+    melody.append((freq, duration))
 
-    for _ in range(length):
-        freq = random.choice(frequencies)
-        duration = random.choice([0.125, 0.25, 0.5])  # Add more duration options for variation
-        melody.append((freq, duration))
+  return melody
 
-    return melody
 
 def generate_drum_pattern(length):
-    bass_drum_freq = 55  # A1 frequency - this will act as our bass drum
-    drum_silence = None
-    drum_pattern = []
-
-    for _ in range(length):
-        if random.random() < 0.4:  # 40% chance of a bass drum hit
-            drum_pattern.append([bass_drum_freq])
-        else:
-            drum_pattern.append(drum_silence)
-
-    return drum_pattern
-
-def random(length = 120)
-    c_major_pentatonic = [261.63, 293.66, 329.63, 392.00, 440.00]  # C4, D4, E4, G4, A4
-    g_major_pentatonic = [392.00, 440.00, 493.88, 587.33, 659.25]  # G4, A4, B4, D5, E5
-    e_minor_pentatonic = [329.63, 392.00, 440.00, 493.88, 587.33]  # E4, G4, A4, B4, D5
-
-    scales = [c_major_pentatonic, g_major_pentatonic, e_minor_pentatonic]
-    scale = random.choice(scales)
-
-    melody_length = length  # Increase the length to make it faster
-    melody1 = generate_melody(scale, melody_length)
-    melody2 = generate_melody(scale, melody_length)
-
-    drum_pattern = generate_drum_pattern(melody_length)
-
-    for idx in range(melody_length):
-        note1, duration1 = melody1[idx]
-        note2, duration2 = melody2[idx]
-        drum = drum_pattern[idx]
+  bass_drum_freq = 55  # A1 frequency - this will act as our bass drum
+  drum_silence = None
+  drum_pattern = []
+
+  for _ in range(length):
+    if random.random() < 0.4:  # 40% chance of a bass drum hit
+      drum_pattern.append([bass_drum_freq])
+    else:
+      drum_pattern.append(drum_silence)
+
+  return drum_pattern
+
+
+def random(length=120):
+  c_major_pentatonic = [261.63, 293.66, 329.63, 392.00,
+                        440.00]  # C4, D4, E4, G4, A4
+  g_major_pentatonic = [392.00, 440.00, 493.88, 587.33,
+                        659.25]  # G4, A4, B4, D5, E5
+  e_minor_pentatonic = [329.63, 392.00, 440.00, 493.88,
+                        587.33]  # E4, G4, A4, B4, D5
+
+  scales = [c_major_pentatonic, g_major_pentatonic, e_minor_pentatonic]
+  scale = random.choice(scales)
+
+  melody_length = length  # Increase the length to make it faster
+  melody1 = generate_melody(scale, melody_length)
+  melody2 = generate_melody(scale, melody_length)
+
+  drum_pattern = generate_drum_pattern(melody_length)
+
+  for idx in range(melody_length):
+    note1, duration1 = melody1[idx]
+    note2, duration2 = melody2[idx]
+    drum = drum_pattern[idx]
 
-        play_notes([note1] or [] + drum or [], duration1)
-        play_notes([note2] or [] + drum or [], duration2)
+    play_notes([note1] or [] + drum or [], duration1)
+    play_notes([note2] or [] + drum or [], duration2)
```

### Comparing `openai_rev-1.0/openai_rev.egg-info/PKG-INFO` & `openai_rev-1.1/openai_rev.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-rev
-Version: 1.0
+Version: 1.1
 Summary: making music with OpenAI (GPT-4)
 Author: bobbill
 License: Unlicense
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```


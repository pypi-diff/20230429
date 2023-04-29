# Comparing `tmp/whisper-ctranslate2-0.2.2.tar.gz` & `tmp/whisper-ctranslate2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.2.tar", last modified: Thu Apr 27 16:19:17 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.3.tar", last modified: Sat Apr 29 09:55:50 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.2.tar` & `whisper-ctranslate2-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.2/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.2/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 15:43:27.000000 whisper-ctranslate2-0.2.2/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4888 2023-04-27 16:15:31.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-27 15:53:01.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-27 15:44:12.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15611 2023-04-27 16:15:31.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5803 2023-04-27 11:52:25.000000 whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-27 16:19:17.724616 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-27 16:19:17.000000 whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.3/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.3/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 15:43:27.000000 whisper-ctranslate2-0.2.3/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4888 2023-04-28 15:31:31.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-29 07:49:33.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-27 16:20:26.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16957 2023-04-29 09:50:29.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10108 2023-04-29 09:43:21.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.2/LICENSE` & `whisper-ctranslate2-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.2/PKG-INFO` & `whisper-ctranslate2-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.2.2/README.md` & `whisper-ctranslate2-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.2/setup.py` & `whisper-ctranslate2-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/live.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 from .transcribe import Transcribe, TranscriptionOptions
 from typing import Union, List
 
 SampleRate = 16000  # Stream device recording frequency per second
 BlockSize = 30  # Block size in milliseconds
-Threshold = 0.2  # Minimum volume threshold to activate listening
 Vocals = [50, 1000]  # Frequency range to detect sounds that could be speech
 EndBlocks = 33 * 2  # Number of blocks to wait before sending (30 ms is block)
 FlushBlocks = 33 * 10  # Number of blocks to wait before sending
 
 try:
     import sounddevice as sd
 
@@ -30,26 +29,28 @@
         task: str,
         language: str,
         threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
         verbose: bool,
+        threshold: float,
         options: TranscriptionOptions,
     ):
         self.model_path = model_path
         self.cache_directory = cache_directory
         self.local_files_only = local_files_only
         self.task = task
         self.language = language
         self.threads = threads
         self.device = device
         self.device_index = device_index
         self.compute_type = compute_type
         self.verbose = verbose
+        self.threshold = threshold
         self.options = options
 
         self.running = True
         self.waiting = 0
         self.prevblock = self.buffer = np.zeros((0, 1))
         self.speaking = False
         self.blocks_speaking = 0
@@ -63,15 +64,15 @@
     def force_not_available_exception():
         raise (sounddevice_exception)
 
     def _is_there_voice(self, indata, frames):
         freq = np.argmax(np.abs(np.fft.rfft(indata[:, 0]))) * SampleRate / frames
         volume = np.sqrt(np.mean(indata**2))
 
-        return volume > Threshold and Vocals[0] <= freq <= Vocals[1]
+        return volume > self.threshold and Vocals[0] <= freq <= Vocals[1]
 
     def _save_to_process(self):
         self.buffers_to_process.append(self.buffer.copy())
         self.buffer = np.zeros((0, 1))
         self.speaking = False
 
     def callback(self, indata, frames, _time, status):
```

### Comparing `whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.2/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,15 +114,28 @@
         help="whether to print out the progress and debug messages",
     )
 
     outputs_args.add_argument(
         "--highlight_words",
         type=str2bool,
         default=False,
-        help="underline each word as it is spoken in srt and vtt (requires --word_timestamps True)",
+        help="underline each word as it is spoken in srt and vtt output formats (requires --word_timestamps True)",
+    )
+
+    outputs_args.add_argument(
+        "--max_line_width",
+        type=optional_int,
+        default=None,
+        help="the maximum number of characters in a line before breaking the line in srt and vtt output formats (requires --word_timestamps True)",
+    )
+    outputs_args.add_argument(
+        "--max_line_count",
+        type=optional_int,
+        default=None,
+        help="the maximum number of lines in a segment in srt and vtt output formats (requires --word_timestamps True)",
     )
 
     computing_args = parser.add_argument_group("Computing configuration options")
 
     computing_args.add_argument(
         "--device",
         choices=[
@@ -314,16 +327,25 @@
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="show program's version number and exit",
     )
 
-    parser.add_argument(
-        "--live_transcribe", type=str2bool, default=False, help="Live transcribe mode"
+    live_args = parser.add_argument_group("Live transcribe options")
+
+    live_args.add_argument(
+        "--live_transcribe", type=str2bool, default=False, help="live transcribe mode"
+    )
+
+    live_args.add_argument(
+        "--live_volume_threshold",
+        type=float,
+        default=0.2,
+        help="minimum volume threshold to activate listening in live transcribe mode",
     )
 
     return parser.parse_args().__dict__
 
 
 def _does_old_cache_dir_has_files():
     default = os.path.join(os.path.expanduser("~"), ".cache")
@@ -348,16 +370,15 @@
     model_directory: str = args.pop("model_directory")
     cache_directory: str = args.pop("model_dir")
     device_index: Union[int, List[int]] = args.pop("device_index")
     suppress_tokens: str = args.pop("suppress_tokens")
     live_transcribe: bool = args.pop("live_transcribe")
     audio: str = args.pop("audio")
     local_files_only: bool = args.pop("local_files_only")
-    highlight_words: bool = args.pop("highlight_words")
-
+    live_volume_threshold: float = args.pop("live_volume_threshold")
     temperature = args.pop("temperature")
     if (increment := args.pop("temperature_increment_on_fallback")) is not None:
         temperature = tuple(np.arange(temperature, 1.0 + 1e-6, increment))
     else:
         temperature = [temperature]
 
     language = from_language_to_iso_code(language)
@@ -400,35 +421,49 @@
     if not live_transcribe and len(audio) == 0:
         sys.stderr.write("You need to specify one or more audio files\n")
         sys.stderr.write(
             "Use `whisper-ctranslate2 --help` to see the available options.\n"
         )
         return
 
-    if not options.word_timestamps and highlight_words:
-        sys.stderr.write("--highlight_words requires --word_timestamps True\n")
-        return
+    word_options = ["highlight_words", "max_line_count", "max_line_width"]
+    if not options.word_timestamps:
+        for option in word_options:
+            if args[option]:
+                sys.stderr.write(f"--{option} requires --word_timestamps True\n")
+                return
+
+    if args["max_line_count"] and not args["max_line_width"]:
+        warnings.warn("--max_line_count has no effect without --max_line_width")
+
+    writer_args = {arg: args.pop(arg) for arg in word_options}
 
     if verbose:
         cache_dir, exists = _does_old_cache_dir_has_files()
         if exists:
             print(
                 f"There are old cache files at `{cache_dir}` which are no longer used. Consider deleting them"
             )
 
     if not verbose and options.print_colors:
-        raise RuntimeError("You cannot disable verbose and enable print colors")
+        sys.stderr.write("You cannot disable verbose and enable print colors\n")
+        return
 
     if live_transcribe and not Live.is_available():
         Live.force_not_available_exception()
 
     if verbose and not language:
-        print(
-            "Detecting language using up to the first 30 seconds. Use `--language` to specify the language"
-        )
+        if live_transcribe:
+            print(
+                "Consider specifying the language using `--language`. It improves significantly prediction in live transcription."
+            )
+        else:
+            print(
+                "Detecting language using up to the first 30 seconds. Use `--language` to specify the language"
+            )
 
     if options.print_colors and output_dir and not options.word_timestamps:
         print(
             "Print colors requires word-level time stamps. Generated files in output directory will have word-level timestamps"
         )
 
     output_dir = os.path.abspath(output_dir)
@@ -448,21 +483,20 @@
             task,
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
+            live_volume_threshold,
             options,
         ).inference()
 
         return
 
-    writer_args = {"highlight_words": highlight_words}
-
     for audio_path in audio:
         result = Transcribe().inference(
             audio_path,
             model_dir,
             cache_directory,
             local_files_only,
             task,
```

### Comparing `whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.2
+Version: 0.2.3
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.2.2/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


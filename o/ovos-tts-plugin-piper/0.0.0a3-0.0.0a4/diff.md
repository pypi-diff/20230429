# Comparing `tmp/ovos_tts_plugin_piper-0.0.0a3-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_piper-0.0.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10969 bytes, number of entries: 10
--rw-r--r--  2.0 unx    11569 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/__init__.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/engine.py
--rw-r--r--  2.0 unx      178 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      948 b- defN 23-Apr-28 04:45 ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD
-10 files, 29928 bytes uncompressed, 9309 bytes compressed:  68.9%
+Zip file size: 10987 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    11651 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper/__init__.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper/engine.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      948 b- defN 23-Apr-28 15:45 ovos_tts_plugin_piper-0.0.0a4.dist-info/RECORD
+10 files, 30010 bytes uncompressed, 9327 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: ovos_tts_plugin_piper/engine.py
 Comment: 
 
 Filename: ovos_tts_plugin_piper/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD
+Filename: ovos_tts_plugin_piper-0.0.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_piper/__init__.py

```diff
@@ -6,23 +6,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import os
+import tarfile
+
 import requests
 from ovos_plugin_manager.templates.g2p import Grapheme2PhonemePlugin
 from ovos_plugin_manager.templates.tts import TTS
-import os
-from ovos_tts_plugin_piper.engine import Piper
+from ovos_utils.log import LOG
 from ovos_utils.xdg_utils import xdg_data_home
-import tarfile
 
-from ovos_utils.log import LOG
+from ovos_tts_plugin_piper.engine import Piper
 
 
 class PiperG2P(Grapheme2PhonemePlugin):
     piper = None
 
     def __init__(self, piper_engine, *args, **kwargs):
         self.piper = piper_engine
@@ -196,17 +197,17 @@
         return wav_file, phonemes
 
     def available_languages(self) -> set:
         return set(self.lang2voices.keys())
 
 
 PiperTTSPluginConfig = {
-    # TODO - list of all models + url + auto download if needed to XDG path
+    lang: [{v: {"model": PiperTTSPlugin.voice2url[v], "offline": True}}
+           for v in voices]
+    for lang, voices in PiperTTSPlugin.lang2voices.items()
 }
 
 if __name__ == "__main__":
-
-
     config = {}
     config["model"] = "alan-low"
     e = PiperTTSPlugin(config=config)
     e.get_tts("hello world", "hello.wav")
```

## ovos_tts_plugin_piper/version.py

```diff
@@ -1,8 +1,8 @@
 
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE` & `ovos_tts_plugin_piper-0.0.0a4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA` & `ovos_tts_plugin_piper-0.0.0a4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-piper
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: piper tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-piper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD` & `ovos_tts_plugin_piper-0.0.0a4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ovos_tts_plugin_piper/__init__.py,sha256=zqb_9ZhEdX7CLSPBv2Aml40dfK-V5R6toHsIgm4b4G0,11569
+ovos_tts_plugin_piper/__init__.py,sha256=l-GECFE8N60rR9Wn95eZKFglSNFnMmFR6hFw_FEC4pI,11651
 ovos_tts_plugin_piper/engine.py,sha256=WEB-2Uu9cmN3UQrltWYbB0PH1H0X03Fg6OnGXW-GS0s,4518
-ovos_tts_plugin_piper/version.py,sha256=XnMBjlWuu_KTmVhM03VIPZxO-m0dNEV7U3SwDK8Amyg,178
-ovos_tts_plugin_piper-0.0.0a3.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_piper-0.0.0a3.dist-info/METADATA,sha256=umyOFFxfY6HYpq5SQTnhduGFUOhuN4p-8gINhzOFJYE,1065
-ovos_tts_plugin_piper-0.0.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_piper-0.0.0a3.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
-ovos_tts_plugin_piper-0.0.0a3.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
-ovos_tts_plugin_piper-0.0.0a3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_piper-0.0.0a3.dist-info/RECORD,,
+ovos_tts_plugin_piper/version.py,sha256=cIGUQx3ZPYxd5qcxEPut9-d-IBg4ucXJzcFaw_hUvZ4,178
+ovos_tts_plugin_piper-0.0.0a4.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_piper-0.0.0a4.dist-info/METADATA,sha256=SMkTxuBubBwxtVjzg8ko6NSDQoNW-renHjmFDIFaAuA,1065
+ovos_tts_plugin_piper-0.0.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_piper-0.0.0a4.dist-info/entry_points.txt,sha256=eHpADEdMHzf8Y-h30EKm587TkxMsv91Xb98ph3DgRUY,186
+ovos_tts_plugin_piper-0.0.0a4.dist-info/top_level.txt,sha256=WTvxxS42UAwh0oi25ypLaxvMGD85j_wGzrux2QFoqLs,22
+ovos_tts_plugin_piper-0.0.0a4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_piper-0.0.0a4.dist-info/RECORD,,
```


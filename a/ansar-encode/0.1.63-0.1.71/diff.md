# Comparing `tmp/ansar-encode-0.1.63.tar.gz` & `tmp/ansar-encode-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.63.tar", last modified: Mon Apr 17 20:34:44 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.71.tar", last modified: Sat Apr 29 21:25:25 2023, max compression
```

## Comparing `ansar-encode-0.1.63.tar` & `ansar-encode-0.1.71.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2022-10-03 18:49:48.000000 ansar-encode-0.1.63/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2022-10-02 23:59:34.000000 ansar-encode-0.1.63/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2022-10-03 00:32:14.000000 ansar-encode-0.1.63/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-01-05 21:34:37.000000 ansar-encode-0.1.63/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-02-04 16:29:11.000000 ansar-encode-0.1.63/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4911 2023-04-17 20:34:40.000000 ansar-encode-0.1.63/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-17 19:54:59.000000 ansar-encode-0.1.63/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-02-28 08:57:41.000000 ansar-encode-0.1.63/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-01-19 23:29:20.000000 ansar-encode-0.1.63/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-15 02:45:44.000000 ansar-encode-0.1.63/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2022-10-03 19:30:53.000000 ansar-encode-0.1.63/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-02-28 08:58:39.000000 ansar-encode-0.1.63/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-02-05 20:30:57.000000 ansar-encode-0.1.63/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2022-09-05 20:25:39.000000 ansar-encode-0.1.63/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6155 2023-02-28 09:06:13.000000 ansar-encode-0.1.63/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2022-10-25 02:07:57.000000 ansar-encode-0.1.63/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2022-08-03 00:49:03.000000 ansar-encode-0.1.63/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4913 2023-04-29 21:25:22.000000 ansar-encode-0.1.71/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.71/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.71/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-29 21:25:25.167003 ansar-encode-0.1.71/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-04-29 21:25:25.000000 ansar-encode-0.1.71/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.63/LICENSE` & `ansar-encode-0.1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/PKG-INFO` & `ansar-encode-0.1.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.63
+Version: 0.1.71
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.63/README.md` & `ansar-encode-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/setup.py` & `ansar-encode-0.1.71/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/command/show_release.py` & `ansar-encode-0.1.71/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/__init__.py` & `ansar-encode-0.1.71/src/ansar/encode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
-Repo: git@ansar.gitlab.com:scott-ansar/ansar-encode.git
+Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: ace301a25c9df66a00df24f4f57e607fbc2591d9
-Version: 0.1.62 (2023-04-18@08:34:40+NZST)
+Commit: f414395799da108c69abeb2ec79fcc978eccde59
+Version: 0.1.70 (2023-04-30@09:25:22+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
@@ -49,15 +49,15 @@
 from .portable import is_portable, is_container, is_structural, is_portable_class, is_container_class
 from .portable import NO_SUCH_ADDRESS
 from .portable import is_address, address_on_proxy
 from .portable import deque
 
 from .runtime import USER_LOG_FAULT, USER_LOG_WARNING, USER_LOG_CONSOLE, USER_LOG_OBJECT, USER_LOG_TRACE, USER_LOG_DEBUG, USER_LOG_NONE
 from .runtime import TAG_CREATED, TAG_DESTROYED, TAG_SENT, TAG_RECEIVED, TAG_STARTED, TAG_ENDED
-from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG
+from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG, TAG_CHECK
 from .runtime import tag_to_number
 from .runtime import Runtime
 from .runtime import CodingProblem, PlatformFailure
 
 from .message import MessageError, MessageRegistrationError
 from .message import Message, is_message, is_message_class
 from .message import Unknown, Incognito
```

### Comparing `ansar-encode-0.1.63/src/ansar/encode/codec.py` & `ansar-encode-0.1.71/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/convert.py` & `ansar-encode-0.1.71/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/file.py` & `ansar-encode-0.1.71/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/folder.py` & `ansar-encode-0.1.71/src/ansar/encode/folder.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/json.py` & `ansar-encode-0.1.71/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/message.py` & `ansar-encode-0.1.71/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/portable.py` & `ansar-encode-0.1.71/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/release.py` & `ansar-encode-0.1.71/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/runtime.py` & `ansar-encode-0.1.71/src/ansar/encode/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     'TAG_ENDED',
 
     'TAG_FAULT',
     'TAG_WARNING',
     'TAG_CONSOLE',
     'TAG_TRACE',
     'TAG_DEBUG',
+    'TAG_CHECK',
 
     'tag_to_number',
 
     'Runtime',
     'CodingProblem',
     'PlatformFailure',
 ]
@@ -86,17 +87,19 @@
 TAG_FAULT     = '!'     # Compromised.
 TAG_WARNING   = '?'     # May be compromised.
 TAG_CONSOLE   = '^'     # Application milestone.
 
 TAG_TRACE     = '~'     # Technical, networks, files and devices.
 TAG_DEBUG     = '_'     # Developer, raw.
 
+TAG_CHECK     = '='		# Check a condition.
+
 TAG_LEVEL = {
     TAG_FAULT: USER_LOG_FAULT,
-    TAG_WARNING: USER_LOG_WARNING,
+    TAG_WARNING: USER_LOG_WARNING, TAG_CHECK: USER_LOG_WARNING,
     TAG_CONSOLE: USER_LOG_CONSOLE,
     TAG_CREATED: USER_LOG_OBJECT, TAG_DESTROYED: USER_LOG_OBJECT, TAG_SENT: USER_LOG_OBJECT, TAG_RECEIVED: USER_LOG_OBJECT,
     TAG_STARTED: USER_LOG_OBJECT, TAG_ENDED: USER_LOG_OBJECT,
     TAG_TRACE: USER_LOG_TRACE,
     TAG_DEBUG: USER_LOG_DEBUG
 }
```

### Comparing `ansar-encode-0.1.63/src/ansar/encode/version.py` & `ansar-encode-0.1.71/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar/encode/xml.py` & `ansar-encode-0.1.71/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.63/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.71/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.63
+Version: 0.1.71
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.63/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.71/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*


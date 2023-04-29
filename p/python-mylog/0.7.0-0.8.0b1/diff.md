# Comparing `tmp/python-mylog-0.7.0.tar.gz` & `tmp/python-mylog-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mylog-0.7.0.tar", last modified: Sun Mar 19 18:32:30 2023, max compression
+gzip compressed data, was "python-mylog-0.8.0b1.tar", last modified: Sat Apr 29 13:13:55 2023, max compression
```

## Comparing `python-mylog-0.7.0.tar` & `python-mylog-0.8.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:30.916613 python-mylog-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-19 18:32:18.000000 python-mylog-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-19 18:32:30.916613 python-mylog-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-19 18:32:18.000000 python-mylog-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-19 18:32:18.000000 python-mylog-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-19 18:32:30.920613 python-mylog-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-19 18:32:18.000000 python-mylog-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:30.912613 python-mylog-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:30.912613 python-mylog-0.7.0/src/mylog/
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-03-19 18:32:18.000000 python-mylog-0.7.0/src/mylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:18.000000 python-mylog-0.7.0/src/mylog/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:30.916613 python-mylog-0.7.0/src/python_mylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 18:32:30.000000 python-mylog-0.7.0/src/python_mylog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:32:30.916613 python-mylog-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-03-19 18:32:18.000000 python-mylog-0.7.0/tests/test_mylog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.725706 python-mylog-0.8.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.733706 python-mylog-0.8.0b1/src/mylog/
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/src/mylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/src/mylog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/src/python_mylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 13:13:55.000000 python-mylog-0.8.0b1/src/python_mylog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:13:55.737707 python-mylog-0.8.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-04-29 13:13:42.000000 python-mylog-0.8.0b1/tests/test_mylog.py
```

### Comparing `python-mylog-0.7.0/LICENSE` & `python-mylog-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mylog-0.7.0/PKG-INFO` & `python-mylog-0.8.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mylog
-Version: 0.7.0
+Version: 0.8.0b1
 Summary: My logger library.
 Home-page: https://github.com/koviubi56/mylog
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: LGPL-3.0
 Project-URL: Release notes, https://github.com/koviubi56/mylog/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/koviubi56/mylog
```

### Comparing `python-mylog-0.7.0/README.md` & `python-mylog-0.8.0b1/README.md`

 * *Files identical despite different names*

### Comparing `python-mylog-0.7.0/pyproject.toml` & `python-mylog-0.8.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-mylog-0.7.0/setup.cfg` & `python-mylog-0.8.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-mylog-0.7.0/src/mylog/__init__.py` & `python-mylog-0.8.0b1/src/mylog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # ruff: noqa: SLF001
 
-__version__ = "0.7.0"
+__version__ = "0.8.0-beta.1"
 
 import abc
 import contextlib
 import dataclasses
 import datetime
 import sys
 import time
@@ -526,20 +526,20 @@
             tb=bool(tb),
         )
         self.list.append(event)
         for handler in self.handlers:
             handler.handle(self, event)
         return event
 
-    def _log(
+    def log(
         self,
         lvl: Levelable,
         msg: Stringable,
-        traceback: bool,
-        frame_depth: int,
+        traceback: bool = False,
+        frame_depth: int = 3,
     ) -> Optional[LogEvent]:
         """
         Log the message. Checks if the logger is enabled, propagate, and stuff.
         This IS in the public api, but (unless you need it) use the methods
         debug, info, warning, error, critical.
 
         Args:
@@ -563,15 +563,15 @@
                     "Root logger should not propagate! Set enabled to"
                     " False if you want to disable it.",
                     UserWarning,
                     stacklevel=frame_depth - 1,
                 )
                 return None
             # Log with parent
-            return self.higher._log(lvl, msg, traceback, frame_depth + 1)
+            return self.higher.log(lvl, msg, traceback, frame_depth + 1)
         # Check if it's enabled
         if not self.is_enabled_for(lvl):
             return None
         # Log
         return self._actually_log(lvl, msg, frame_depth, traceback)
 
     def debug(
@@ -584,15 +584,15 @@
             msg (Stringable): The message.
             traceback (bool, optional): Whether to include the traceback.\
  Defaults to False.
 
         Returns:
             int: The number of characters written.
         """
-        return self._log(Level.debug, msg, traceback, 5)
+        return self.log(Level.debug, msg, traceback, 5)
 
     def info(
         self, msg: Stringable, traceback: bool = False
     ) -> Optional[LogEvent]:
         """
         Log an info message.
 
@@ -600,15 +600,15 @@
             msg (Stringable): The message.
             traceback (bool, optional): Whether to include the traceback.\
  Defaults to False.
 
         Returns:
             int: The number of characters written.
         """
-        return self._log(Level.info, msg, traceback, 5)
+        return self.log(Level.info, msg, traceback, 5)
 
     def warning(
         self, msg: Stringable, traceback: bool = False
     ) -> Optional[LogEvent]:
         """
         Log a warning message.
 
@@ -616,15 +616,15 @@
             msg (Stringable): The message.
             traceback (bool, optional): Whether to include the traceback.\
  Defaults to False.
 
         Returns:
             int: The number of characters written.
         """
-        return self._log(Level.warning, msg, traceback, 5)
+        return self.log(Level.warning, msg, traceback, 5)
 
     def error(
         self, msg: Stringable, traceback: bool = False
     ) -> Optional[LogEvent]:
         """
         Log an error message.
 
@@ -632,15 +632,15 @@
             msg (Stringable): The message.
             traceback (bool, optional): Whether to include the traceback.\
  Defaults to False.
 
         Returns:
             int: The number of characters written.
         """
-        return self._log(Level.error, msg, traceback, 5)
+        return self.log(Level.error, msg, traceback, 5)
 
     def critical(
         self, msg: Stringable, traceback: bool = False
     ) -> Optional[LogEvent]:
         """
         Log a critical/fatal message.
 
@@ -648,15 +648,15 @@
             msg (Stringable): The message.
             traceback (bool, optional): Whether to include the traceback.\
  Defaults to False.
 
         Returns:
             int: The number of characters written.
         """
-        return self._log(Level.critical, msg, traceback, 5)
+        return self.log(Level.critical, msg, traceback, 5)
 
     def get_child(self, name: str) -> "Logger":
         """
         Get a child logger.
 
         Returns:
             Logger: The child logger.
```

### Comparing `python-mylog-0.7.0/src/python_mylog.egg-info/PKG-INFO` & `python-mylog-0.8.0b1/src/python_mylog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mylog
-Version: 0.7.0
+Version: 0.8.0b1
 Summary: My logger library.
 Home-page: https://github.com/koviubi56/mylog
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: LGPL-3.0
 Project-URL: Release notes, https://github.com/koviubi56/mylog/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/koviubi56/mylog
```

### Comparing `python-mylog-0.7.0/tests/test_mylog.py` & `python-mylog-0.8.0b1/tests/test_mylog.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,15 +489,15 @@
         logger.higher.handlers = []
         logger.higher.threshold = mylog.Level.debug
         lvl = _random_level()
         msg = random_anything()
         frame_depth = _randint(0, 3)
 
         time = get_unix_time()
-        logger._log(lvl[0], msg, False, frame_depth)
+        logger.log(lvl[0], msg, False, frame_depth)
 
         assert not logger.list
         event = logger.higher.list[-1]
         assert event.msg == str(msg)
         assert event.level == lvl[1]
         assert time - 1 < event.time < time + 1
         assert event.indent == logger.higher.indent
@@ -506,30 +506,30 @@
         # Since propagate is True, Logger._log() will automatically add one to
         # the frame_depth, if logging is done by the parent.
 
         with pytest.warns(
             UserWarning, match="Root logger should not propagate"
         ):
             mylog.root.propagate = True
-            mylog.root._log(_random_level()[0], random_anything(), False, 2)
+            mylog.root.log(_random_level()[0], random_anything(), False, 2)
             mylog.root.propagate = False
 
     @staticmethod
     def test_log_no_propagate():
         logger = mylog.root
         logger.list = []
         logger.indent = _randint(0, 10)
         logger.threshold = mylog.Level.debug
         logger.handlers = []
         lvl = _random_level()
         msg = random_anything()
         frame_depth = _randint(0, 3)
 
         time = get_unix_time()
-        logger._log(lvl[0], msg, False, frame_depth)
+        logger.log(lvl[0], msg, False, frame_depth)
 
         assert len(logger.list) == 1
         event = logger.list[-1]
         assert event.msg == str(msg)
         assert event.level == lvl[1]
         assert time - 1 < event.time < time + 1
         assert event.indent == logger.indent
```


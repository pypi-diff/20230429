# Comparing `tmp/fastf1-2.3.2.tar.gz` & `tmp/fastf1-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-2.3.2.tar", last modified: Thu Apr  6 08:32:13 2023, max compression
+gzip compressed data, was "fastf1-2.3.3.tar", last modified: Sat Apr 29 11:23:21 2023, max compression
```

## Comparing `fastf1-2.3.2.tar` & `fastf1-2.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:32:13.455727 fastf1-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 08:32:02.000000 fastf1-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-06 08:32:02.000000 fastf1-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-06 08:32:13.455727 fastf1-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-06 08:32:02.000000 fastf1-2.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:32:13.455727 fastf1-2.3.2/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70728 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   118447 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/ergast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:32:13.455727 fastf1-2.3.2/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 08:32:02.000000 fastf1-2.3.2/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:32:13.455727 fastf1-2.3.2/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 08:32:13.000000 fastf1-2.3.2/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 08:32:02.000000 fastf1-2.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-06 08:32:13.455727 fastf1-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-06 08:32:02.000000 fastf1-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 11:23:10.000000 fastf1-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 11:23:10.000000 fastf1-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-29 11:23:21.499235 fastf1-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-29 11:23:10.000000 fastf1-2.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70728 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118447 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/ergast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30500 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 11:23:10.000000 fastf1-2.3.3/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:23:21.499235 fastf1-2.3.3/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 11:23:21.000000 fastf1-2.3.3/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 11:23:10.000000 fastf1-2.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 11:23:21.499235 fastf1-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 11:23:10.000000 fastf1-2.3.3/setup.py
```

### Comparing `fastf1-2.3.2/LICENSE` & `fastf1-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/PKG-INFO` & `fastf1-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 2.3.2
+Version: 2.3.3
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: =======
         Fast F1
```

### Comparing `fastf1-2.3.2/README.rst` & `fastf1-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/__init__.py` & `fastf1-2.3.3/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/api.py` & `fastf1-2.3.3/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/core.py` & `fastf1-2.3.3/fastf1/core.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/ergast.py` & `fastf1-2.3.3/fastf1/ergast.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/events.py` & `fastf1-2.3.3/fastf1/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     Usually, this is the same as the date of the last session.
 
   - ``EventFormat`` | :class:`str` |
     The format of the event. One of 'conventional', 'sprint', 'testing'.
 
   - ``Session*`` | :class:`str` |
     The name of the session. One of 'Practice 1', 'Practice 2', 'Practice 3',
-    'Qualifying', 'Sprint Qualifying' or 'Race'.
+    'Qualifying', 'Sprint Qualifying', 'Sprint Shootout' or 'Race'.
     Testing sessions are considered practice.
     ``*`` denotes the number of
     the session (1, 2, 3, 4, 5).
 
   - ``Session*Date`` | :class:`datetime` |
     The date and time at which the session is scheduled to start or was
     scheduled to start.
@@ -97,19 +97,19 @@
 -------------------
 
 Multiple event (schedule) related functions and methods make use of a session
 identifier to differentiate between the various sessions of one event.
 This identifier can currently be one of the following:
 
     - session name abbreviation: ``'FP1', 'FP2', 'FP3', 'Q', 'S',
-      'SQ', 'R'``
+      'SQ', 'SS', 'R'``
     - full session name: ``'Practice 1', 'Practice 2',
-      'Practice 3', 'Sprint Qualifying', 'Sprint', 'Qualifying', 'Race'``;
-      provided names will be normalized, so that the name is
-      case-insensitive
+      'Practice 3', 'Sprint Qualifying', 'Sprint', 'Sprint Shootout',
+      'Qualifying', 'Race'``;
+      provided names will be normalized, so that the name is case-insensitive
     - number of the session: ``1, 2, 3, 4, 5``
 
 Note that 'Sprint' is called 'Sprint Qualifying' only in the 2021 season.
 The event name will silently be corrected if you use 'Sprint'/'S' for the 2021
 season or 'Sprint Qualifying'/'SQ' for the subsequent seasons.
 
 
@@ -175,14 +175,15 @@
 
 
 _SESSION_TYPE_ABBREVIATIONS = {
     'R': 'Race',
     'Q': 'Qualifying',
     'S': 'Sprint',
     'SQ': 'Sprint Qualifying',
+    'SS': 'Sprint Shootout',
     'FP1': 'Practice 1',
     'FP2': 'Practice 2',
     'FP3': 'Practice 3'
 }
 
 _SCHEDULE_BASE_URL = "https://raw.githubusercontent.com/" \
                      "theOehrly/f1schedule/master/"
@@ -762,17 +763,15 @@
                 try:
                     session_name = \
                         _SESSION_TYPE_ABBREVIATIONS[identifier.upper()]
                 except KeyError:
                     raise ValueError(f"Invalid session type '{identifier}'")
 
             # 'Sprint' is called 'Sprint Qualifying' only in 2021
-            if (self.year == 2021) and (session_name == 'Sprint'):
-                session_name = 'Sprint Qualifying'
-            elif (self.year > 2021) and (session_name == 'Sprint Qualifying'):
+            if session_name == 'Sprint Qualifying':
                 session_name = 'Sprint'
 
             if session_name not in self.values:
                 raise ValueError(f"Session type '{identifier}' does not "
                                  f"exist for this event")
         else:
             # by number
@@ -869,15 +868,19 @@
         """Return the sprint session.
 
         Returns:
             :class:`Session` instance
         """
         return self.get_session('Sprint')
 
-    def get_practice(self, number):
+    def get_sprint_shootout(self) -> "Session":
+        """Return the sprint shootout session."""
+        return self.get_session('Sprint Shootout')
+
+    def get_practice(self, number: int) -> "Session":
         """Return the specified practice session.
         Args:
             number: 1, 2 or 3 - Free practice session number
         Returns:
             :class:`Session` instance
         """
         return self.get_session(f'Practice {number}')
```

### Comparing `fastf1-2.3.2/fastf1/legacy.py` & `fastf1-2.3.3/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/livetiming/__init__.py` & `fastf1-2.3.3/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/livetiming/__main__.py` & `fastf1-2.3.3/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/livetiming/client.py` & `fastf1-2.3.3/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/livetiming/data.py` & `fastf1-2.3.3/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/plotting.py` & `fastf1-2.3.3/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1/utils.py` & `fastf1-2.3.3/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/fastf1.egg-info/PKG-INFO` & `fastf1-2.3.3/fastf1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 2.3.2
+Version: 2.3.3
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: =======
         Fast F1
```

### Comparing `fastf1-2.3.2/fastf1.egg-info/SOURCES.txt` & `fastf1-2.3.3/fastf1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastf1-2.3.2/setup.cfg` & `fastf1-2.3.3/setup.cfg`

 * *Files identical despite different names*


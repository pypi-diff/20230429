# Comparing `tmp/FindSystemFontsFilename-0.0.2.tar.gz` & `tmp/FindSystemFontsFilename-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindSystemFontsFilename-0.0.2.tar", last modified: Sat Apr 29 02:46:03 2023, max compression
+gzip compressed data, was "FindSystemFontsFilename-0.0.3.tar", last modified: Sat Apr 29 13:33:34 2023, max compression
```

## Comparing `FindSystemFontsFilename-0.0.2.tar` & `FindSystemFontsFilename-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.733648 FindSystemFontsFilename-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.721254 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/
--rw-rw-rw-   0        0        0     1984 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1984 2023-04-29 02:46:03.732670 FindSystemFontsFilename-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.731017 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/
--rw-rw-rw-   0        0        0      140 2023-04-29 02:32:48.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/exceptions.py
--rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/fonts_filename.py
--rw-rw-rw-   0        0        0     4441 2023-04-28 16:05:18.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/linux_fonts.py
--rw-rw-rw-   0        0        0     4673 2023-04-29 02:31:37.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/mac_fonts.py
--rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/system_fonts.py
--rw-rw-rw-   0        0        0    20206 2023-04-28 16:04:31.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/windows_fonts.py
--rw-rw-rw-   0        0        0       42 2023-04-29 02:46:03.733648 FindSystemFontsFilename-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:34.023905 FindSystemFontsFilename-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:33.980882 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/
+-rw-rw-rw-   0        0        0     1984 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 13:33:33.000000 FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1984 2023-04-29 13:33:34.022929 FindSystemFontsFilename-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 13:33:34.020002 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/
+-rw-rw-rw-   0        0        0      140 2023-04-29 13:26:27.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/exceptions.py
+-rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/fonts_filename.py
+-rw-rw-rw-   0        0        0     4441 2023-04-28 16:05:18.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/linux_fonts.py
+-rw-rw-rw-   0        0        0     4681 2023-04-29 13:26:53.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/mac_fonts.py
+-rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/system_fonts.py
+-rw-rw-rw-   0        0        0    20206 2023-04-28 16:04:31.000000 FindSystemFontsFilename-0.0.3/find_system_fonts_filename/windows_fonts.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:33:34.023905 FindSystemFontsFilename-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.3/setup.py
```

### Comparing `FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/PKG-INFO` & `FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
```

### Comparing `FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/SOURCES.txt` & `FindSystemFontsFilename-0.0.3/FindSystemFontsFilename.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/LICENSE` & `FindSystemFontsFilename-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/PKG-INFO` & `FindSystemFontsFilename-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
```

### Comparing `FindSystemFontsFilename-0.0.2/README.md` & `FindSystemFontsFilename-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/fonts_filename.py` & `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/fonts_filename.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/linux_fonts.py` & `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/linux_fonts.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/mac_fonts.py` & `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/mac_fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class MacFonts(SystemFonts):
     _core_foundation = None
     _core_text = None
     # CoreText has an API to get the format of the font: https://developer.apple.com/documentation/coretext/ctfontformat
     # But, the API is "semi-broken" since it says .dfont are TrueType. This is kinda true, but it is not a behaviour that we want.
     # So, we only check the file extension and see if it is valid.
-    VALID_FONT_FORMATS = ["ttf", "ttc", "otf"]
+    VALID_FONT_FORMATS = ["ttf", "otf", "ttc"]
 
     def get_system_fonts_filename() -> Set[str]:
         if MacVersionHelpers.is_mac_version_or_greater(10, 6):
             if MacFonts._core_foundation is None or MacFonts._core_text is None:
                 MacFonts._load_core_library()
 
             fonts_filename = set()
@@ -32,15 +32,15 @@
 
                 file_name_ptr = create_string_buffer(max_length)
                 no_error = MacFonts._core_foundation.CFURLGetFileSystemRepresentation(url, True, file_name_ptr, max_length)
 
                 if no_error:
                     filename = file_name_ptr.value.decode()
 
-                    if Path(filename).suffix.lstrip(".").strip() in MacFonts.VALID_FONT_FORMATS:
+                    if Path(filename).suffix.lstrip(".").strip().lower() in MacFonts.VALID_FONT_FORMATS:
                         fonts_filename.add(filename)
                 else:
                     raise Exception("An unexpected error has occurred while decoded the CFURL.")
 
             MacFonts._core_foundation.CFRelease(font_urls)
         else:
             raise OSNotSupported("FindSystemFontsFilename only works on Mac 10.6 or more")
```

### Comparing `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/windows_fonts.py` & `FindSystemFontsFilename-0.0.3/find_system_fonts_filename/windows_fonts.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.2/setup.py` & `FindSystemFontsFilename-0.0.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/FindSystemFontsFilename-0.0.1.tar.gz` & `tmp/FindSystemFontsFilename-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindSystemFontsFilename-0.0.1.tar", last modified: Fri Apr 28 02:00:48 2023, max compression
+gzip compressed data, was "FindSystemFontsFilename-0.0.2.tar", last modified: Sat Apr 29 02:46:03 2023, max compression
```

## Comparing `FindSystemFontsFilename-0.0.1.tar` & `FindSystemFontsFilename-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 02:00:48.903120 FindSystemFontsFilename-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-28 02:00:48.894256 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/
--rw-rw-rw-   0        0        0     1517 2023-04-28 02:00:48.000000 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2023-04-28 02:00:48.000000 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 02:00:48.000000 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-04-28 02:00:48.000000 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-28 02:00:48.000000 FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1517 2023-04-28 02:00:48.903120 FindSystemFontsFilename-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-04-28 01:53:25.000000 FindSystemFontsFilename-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 02:00:48.901090 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/
--rw-rw-rw-   0        0        0       80 2023-04-28 01:20:51.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/__init__.py
--rw-rw-rw-   0        0        0      607 2023-04-28 01:56:36.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/fonts_filename.py
--rw-rw-rw-   0        0        0     4388 2023-04-28 01:41:48.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/linux_fonts.py
--rw-rw-rw-   0        0        0     1787 2023-04-28 01:56:54.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/mac_fonts.py
--rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/system_fonts.py
--rw-rw-rw-   0        0        0    19802 2023-04-28 01:39:02.000000 FindSystemFontsFilename-0.0.1/find_system_fonts_filename/windows_fonts.py
--rw-rw-rw-   0        0        0       42 2023-04-28 02:00:48.903120 FindSystemFontsFilename-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1763 2023-04-28 01:44:48.000000 FindSystemFontsFilename-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.733648 FindSystemFontsFilename-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.721254 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/
+-rw-rw-rw-   0        0        0     1984 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 02:46:03.000000 FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1984 2023-04-29 02:46:03.732670 FindSystemFontsFilename-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 02:46:03.731017 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/
+-rw-rw-rw-   0        0        0      140 2023-04-29 02:32:48.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/exceptions.py
+-rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/fonts_filename.py
+-rw-rw-rw-   0        0        0     4441 2023-04-28 16:05:18.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/linux_fonts.py
+-rw-rw-rw-   0        0        0     4673 2023-04-29 02:31:37.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/mac_fonts.py
+-rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/system_fonts.py
+-rw-rw-rw-   0        0        0    20206 2023-04-28 16:04:31.000000 FindSystemFontsFilename-0.0.2/find_system_fonts_filename/windows_fonts.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 02:46:03.733648 FindSystemFontsFilename-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.2/setup.py
```

### Comparing `FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/PKG-INFO` & `FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
@@ -17,25 +17,33 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FindSystemFontsFilename
-This tool allows you to get the font filename on your system.
+This tool allows you to get the font filename on your system. It will collect TrueType (.ttf), OpenType (.otf) and TrueType Collection (.ttf) font format.
 
 It uses some APIs to find the font filename:
 - Windows: [DirectWrite API](https://learn.microsoft.com/en-us/windows/win32/directwrite/direct-write-portal)
 - macOS: [Core Text API](https://developer.apple.com/documentation/coretext)
 - Linux: [Fontconfig API](https://www.freedesktop.org/wiki/Software/fontconfig/)
 
 ## Installation
 ```
 pip install FindSystemFontsFilename
 ```
 
 ## How to use it
 ```python
-from find_system_fonts_filename import get_system_fonts_filename
+from find_system_fonts_filename import get_system_fonts_filename, FontConfigNotFound, OSNotSupported
 
-fonts_filename = get_system_fonts_filename()
+try:
+    fonts_filename = get_system_fonts_filename()
+except (FontConfigNotFound, OSNotSupported):
+    # Deal with the exception
+    # OSNotSupported can only happen in Windows and macOS
+    #   - Windows Vista SP2 and more are supported
+    #   - macOS 10.6 and more are supported
+    # FontConfigNotFound can only happen on Linux when Fontconfig could't be found.
+    pass
 ```
```

### Comparing `FindSystemFontsFilename-0.0.1/FindSystemFontsFilename.egg-info/SOURCES.txt` & `FindSystemFontsFilename-0.0.2/FindSystemFontsFilename.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,12 +3,13 @@
 setup.py
 FindSystemFontsFilename.egg-info/PKG-INFO
 FindSystemFontsFilename.egg-info/SOURCES.txt
 FindSystemFontsFilename.egg-info/dependency_links.txt
 FindSystemFontsFilename.egg-info/requires.txt
 FindSystemFontsFilename.egg-info/top_level.txt
 find_system_fonts_filename/__init__.py
+find_system_fonts_filename/exceptions.py
 find_system_fonts_filename/fonts_filename.py
 find_system_fonts_filename/linux_fonts.py
 find_system_fonts_filename/mac_fonts.py
 find_system_fonts_filename/system_fonts.py
 find_system_fonts_filename/windows_fonts.py
```

### Comparing `FindSystemFontsFilename-0.0.1/LICENSE` & `FindSystemFontsFilename-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.1/PKG-INFO` & `FindSystemFontsFilename-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
@@ -17,25 +17,33 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FindSystemFontsFilename
-This tool allows you to get the font filename on your system.
+This tool allows you to get the font filename on your system. It will collect TrueType (.ttf), OpenType (.otf) and TrueType Collection (.ttf) font format.
 
 It uses some APIs to find the font filename:
 - Windows: [DirectWrite API](https://learn.microsoft.com/en-us/windows/win32/directwrite/direct-write-portal)
 - macOS: [Core Text API](https://developer.apple.com/documentation/coretext)
 - Linux: [Fontconfig API](https://www.freedesktop.org/wiki/Software/fontconfig/)
 
 ## Installation
 ```
 pip install FindSystemFontsFilename
 ```
 
 ## How to use it
 ```python
-from find_system_fonts_filename import get_system_fonts_filename
+from find_system_fonts_filename import get_system_fonts_filename, FontConfigNotFound, OSNotSupported
 
-fonts_filename = get_system_fonts_filename()
+try:
+    fonts_filename = get_system_fonts_filename()
+except (FontConfigNotFound, OSNotSupported):
+    # Deal with the exception
+    # OSNotSupported can only happen in Windows and macOS
+    #   - Windows Vista SP2 and more are supported
+    #   - macOS 10.6 and more are supported
+    # FontConfigNotFound can only happen on Linux when Fontconfig could't be found.
+    pass
 ```
```

### Comparing `FindSystemFontsFilename-0.0.1/find_system_fonts_filename/fonts_filename.py` & `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/fonts_filename.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from platform import system
+from .exceptions import OSNotSupported
 
 
 def get_system_fonts_filename():
     system_name = system()
 
     if system_name == "Windows":
         from .windows_fonts import WindowsFonts
@@ -13,8 +14,8 @@
         return LinuxFonts.get_system_fonts_filename()
 
     elif system_name == "Darwin":
         from .mac_fonts import MacFonts
         return MacFonts.get_system_fonts_filename()
 
     else:
-        raise Exception("FindSystemFontsFilename only works on Windows, Mac and Linux.")
+        raise OSNotSupported("FindSystemFontsFilename only works on Windows, Mac and Linux.")
```

### Comparing `FindSystemFontsFilename-0.0.1/find_system_fonts_filename/linux_fonts.py` & `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/linux_fonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ctypes import byref, c_char_p, c_int, c_void_p, cdll, POINTER, Structure, util
 from enum import Enum, IntEnum
 from typing import Set
+from .exceptions import FontConfigNotFound
 from .system_fonts import SystemFonts
 
 
 class FC_FONT_FORMAT(Enum):
     # https://freetype.org/freetype2/docs/reference/ft2-font_formats.html#ft_get_font_format
     # https://gitlab.freedesktop.org/freetype/freetype/-/blob/0a3836c97d5e84d6721ac0fd2839e8ae1b7be8d9/include/freetype/internal/services/svfntfmt.h#L36
     FT_FONT_FORMAT_TRUETYPE = b"TrueType"
@@ -83,15 +84,15 @@
 
 
     @staticmethod
     def _load_font_config_library():
         font_config_library_name = util.find_library("fontconfig")
 
         if font_config_library_name is None:
-            raise Exception("You need to install FontConfig to get the fonts filename")
+            raise FontConfigNotFound("You need to install FontConfig to get the fonts filename")
 
         LinuxFonts._font_config = cdll.LoadLibrary(font_config_library_name)
 
         LinuxFonts._font_config.FcInitLoadConfigAndFonts.restype = c_void_p
         LinuxFonts._font_config.FcInitLoadConfigAndFonts.argtypes = []
 
         LinuxFonts._font_config.FcPatternCreate.restype = c_void_p
```

### Comparing `FindSystemFontsFilename-0.0.1/find_system_fonts_filename/windows_fonts.py` & `FindSystemFontsFilename-0.0.2/find_system_fonts_filename/windows_fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from comtypes import COMError, GUID, HRESULT, IUnknown, STDMETHOD
 from ctypes import byref, create_unicode_buffer, POINTER, windll, wintypes
 from enum import IntEnum
 from sys import getwindowsversion
 from typing import Set
+from .exceptions import OSNotSupported
 from .system_fonts import SystemFonts
 
 
-DWriteCreateFactory = windll.dwrite.DWriteCreateFactory
-DWriteCreateFactory.restype = HRESULT
-DWriteCreateFactory.argtypes = [wintypes.UINT, GUID, POINTER(POINTER(IUnknown))]
-
-
 class DWRITE_FACTORY_TYPE(IntEnum):
     # https://learn.microsoft.com/en-us/windows/win32/api/dwrite/ne-dwrite-dwrite_factory_type
     DWRITE_FACTORY_TYPE_SHARED = 0
     DWRITE_FACTORY_TYPE_ISOLATED = 1
 
 
 class DWRITE_FONT_FILE_TYPE(IntEnum):
@@ -229,14 +225,15 @@
         STDMETHOD(None, "CreateFontCollectionFromFontSet"),  # Need to be implemented
         STDMETHOD(None, "GetSystemFontCollection3"),  # Need to be implemented
         STDMETHOD(None, "GetFontDownloadQueue"),  # Need to be implemented
     ]
 
 
 class WindowsFonts(SystemFonts):
+    _DWriteCreateFactory = None
     VALID_FONT_FORMATS = [
         DWRITE_FONT_FILE_TYPE.DWRITE_FONT_FILE_TYPE_CFF,
         DWRITE_FONT_FILE_TYPE.DWRITE_FONT_FILE_TYPE_TRUETYPE,
         DWRITE_FONT_FILE_TYPE.DWRITE_FONT_FILE_TYPE_OPENTYPE_COLLECTION,
         DWRITE_FONT_FILE_TYPE.DWRITE_FONT_FILE_TYPE_TRUETYPE_COLLECTION,
     ]
 
@@ -244,31 +241,30 @@
         windows_version = getwindowsversion()
 
         if WindowsVersionHelpers.is_windows_10_or_greater(windows_version):
             fonts_filename = WindowsFonts._get_fonts_filename_windows_10_or_more()
         elif WindowsVersionHelpers.is_windows_vista_sp2_or_greater(windows_version):
             fonts_filename = WindowsFonts._get_fonts_filename_windows_vista_sp2_or_more()
         else:
-            raise Exception("FindSystemFontsFilename only works on Windows Vista SP2 or more")
+            raise OSNotSupported("FindSystemFontsFilename only works on Windows Vista SP2 or more")
 
         return fonts_filename
 
     @staticmethod
     def _get_fonts_filename_windows_10_or_more() -> Set[str]:
         """
         Return an set of all the installed fonts filename.
         """
+        if WindowsFonts._DWriteCreateFactory is None:
+            WindowsFonts._load_DWriteCreateFactory()
+
         fonts_filename = set()
 
         dwrite_factory = POINTER(IDWriteFactory3)()
-        DWriteCreateFactory(
-            DWRITE_FACTORY_TYPE.DWRITE_FACTORY_TYPE_ISOLATED,
-            IDWriteFactory3._iid_,
-            byref(dwrite_factory),
-        )
+        WindowsFonts._DWriteCreateFactory(DWRITE_FACTORY_TYPE.DWRITE_FACTORY_TYPE_ISOLATED, IDWriteFactory3._iid_, byref(dwrite_factory))
 
         font_set = POINTER(IDWriteFontSet)()
         dwrite_factory.GetSystemFontSet(byref(font_set))
 
         for i in range(font_set.GetFontCount()):
             font_face_reference = POINTER(IDWriteFontFaceReference)()
             font_set.GetFontFaceReference(i, byref(font_face_reference))
@@ -308,18 +304,21 @@
         return fonts_filename
 
     @staticmethod
     def _get_fonts_filename_windows_vista_sp2_or_more() -> Set[str]:
         """
         Return an set of all the installed fonts filename.
         """
+        if WindowsFonts._DWriteCreateFactory is None:
+            WindowsFonts._load_DWriteCreateFactory()
+
         fonts_filename = set()
 
         dwrite_factory = POINTER(IDWriteFactory)()
-        DWriteCreateFactory(DWRITE_FACTORY_TYPE.DWRITE_FACTORY_TYPE_ISOLATED, IDWriteFactory._iid_, byref(dwrite_factory))
+        WindowsFonts._DWriteCreateFactory(DWRITE_FACTORY_TYPE.DWRITE_FACTORY_TYPE_ISOLATED, IDWriteFactory._iid_, byref(dwrite_factory))
 
         sys_collection = POINTER(IDWriteFontCollection)()
         dwrite_factory.GetSystemFontCollection(byref(sys_collection), False)
 
         for i in range(sys_collection.GetFontFamilyCount()):
             family = POINTER(IDWriteFontFamily)()
             sys_collection.GetFontFamily(i, byref(family))
@@ -364,14 +363,21 @@
 
                     buffer = create_unicode_buffer(path_len.value + 1)
                     local_loader.GetFilePathFromKey(font_file_reference_key, font_file_reference_key_size, buffer, len(buffer))
 
                     fonts_filename.add(buffer.value)
 
         return fonts_filename
+    
+
+    @staticmethod
+    def _load_DWriteCreateFactory():
+        WindowsFonts._DWriteCreateFactory = windll.dwrite.DWriteCreateFactory
+        WindowsFonts._DWriteCreateFactory.restype = HRESULT
+        WindowsFonts._DWriteCreateFactory.argtypes = [wintypes.UINT, GUID, POINTER(POINTER(IUnknown))]
 
 
 class WindowsVersionHelpers:
     @staticmethod
     def is_windows_version_or_greater(windows_version, major: int, minor: int, service_pack_major: int) -> bool:
         """
         Parameters:
```

### Comparing `FindSystemFontsFilename-0.0.1/setup.py` & `FindSystemFontsFilename-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     version=find_version("find_system_fonts_filename", "__init__.py"),
     packages=["find_system_fonts_filename"],
     python_requires=">=3.8",
     install_requires=[
         "comtypes; platform_system=='Windows'",
-        "pyobjc-framework-CoreText; platform_system=='Darwin'",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```


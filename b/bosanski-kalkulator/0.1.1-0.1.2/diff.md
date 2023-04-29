# Comparing `tmp/bosanski_kalkulator-0.1.1.tar.gz` & `tmp/bosanski_kalkulator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosanski_kalkulator-0.1.1.tar", last modified: Wed Feb  8 06:14:47 2023, max compression
+gzip compressed data, was "bosanski_kalkulator-0.1.2.tar", last modified: Sat Apr 29 09:02:16 2023, max compression
```

## Comparing `bosanski_kalkulator-0.1.1.tar` & `bosanski_kalkulator-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.915685 bosanski_kalkulator-0.1.1/
--rw-rw-r--   0 stariki   (1000) stariki   (1000)      126 2023-02-08 06:13:27.000000 bosanski_kalkulator-0.1.1/CHANGELOG.md
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     1091 2023-02-07 12:34:48.000000 bosanski_kalkulator-0.1.1/LICENSE
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     4487 2023-02-08 06:14:47.915685 bosanski_kalkulator-0.1.1/PKG-INFO
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     2394 2023-02-07 23:11:01.000000 bosanski_kalkulator-0.1.1/README.md
--rw-rw-r--   0 stariki   (1000) stariki   (1000)       89 2023-02-07 12:21:55.000000 bosanski_kalkulator-0.1.1/pyproject.toml
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     1181 2023-02-08 06:14:47.919685 bosanski_kalkulator-0.1.1/setup.cfg
--rw-rw-r--   0 stariki   (1000) stariki   (1000)       36 2023-02-07 12:23:42.000000 bosanski_kalkulator-0.1.1/setup.py
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.879686 bosanski_kalkulator-0.1.1/src/
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.879686 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/
--rw-rw-r--   0 stariki   (1000) stariki   (1000)        0 2023-02-07 12:22:03.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/__init__.py
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.915685 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/audio/
--rw-rw-r--   0 stariki   (1000) stariki   (1000)  6915885 2023-02-07 10:23:25.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/audio/bosanska_artiljerija.mp3
--rw-rw-r--   0 stariki   (1000) stariki   (1000)    18104 2023-02-07 11:13:34.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/audio/pucnjava.mp3
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.915685 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/images/
--rw-rw-r--   0 stariki   (1000) stariki   (1000)   220257 2023-02-07 05:51:27.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/images/zastava_bosne_i_hercegovine.png
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     6124 2023-02-07 22:41:07.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/main.py
-drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-02-08 06:14:47.879686 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/
--rw-rw-r--   0 stariki   (1000) stariki   (1000)     4487 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/PKG-INFO
--rw-rw-r--   0 stariki   (1000) stariki   (1000)      577 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/SOURCES.txt
--rw-rw-r--   0 stariki   (1000) stariki   (1000)        1 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/dependency_links.txt
--rw-rw-r--   0 stariki   (1000) stariki   (1000)       61 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/entry_points.txt
--rw-rw-r--   0 stariki   (1000) stariki   (1000)       22 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/requires.txt
--rw-rw-r--   0 stariki   (1000) stariki   (1000)       20 2023-02-08 06:14:47.000000 bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/top_level.txt
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.880305 bosanski_kalkulator-0.1.2/
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)      194 2023-04-29 09:01:56.000000 bosanski_kalkulator-0.1.2/CHANGELOG.md
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     1091 2023-02-07 12:34:48.000000 bosanski_kalkulator-0.1.2/LICENSE
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     4738 2023-04-29 09:02:16.880305 bosanski_kalkulator-0.1.2/PKG-INFO
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     2577 2023-04-29 08:57:07.000000 bosanski_kalkulator-0.1.2/README.md
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)       89 2023-02-07 12:21:55.000000 bosanski_kalkulator-0.1.2/pyproject.toml
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     1181 2023-04-29 09:02:16.880305 bosanski_kalkulator-0.1.2/setup.cfg
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)       36 2023-02-07 12:23:42.000000 bosanski_kalkulator-0.1.2/setup.py
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.840307 bosanski_kalkulator-0.1.2/src/
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.840307 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)        0 2023-02-07 12:22:03.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/__init__.py
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.876305 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/audio/
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)  6915885 2023-02-07 10:23:25.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/audio/bosanska_artiljerija.mp3
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)    18104 2023-02-07 11:13:34.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/audio/pucnjava.mp3
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.876305 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/images/
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)   220257 2023-02-07 05:51:27.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/images/zastava_bosne_i_hercegovine.png
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     6124 2023-02-07 22:41:07.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/main.py
+drwxrwxr-x   0 stariki   (1000) stariki   (1000)        0 2023-04-29 09:02:16.844307 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)     4738 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/PKG-INFO
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)      577 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)        1 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)       61 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/entry_points.txt
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)       22 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/requires.txt
+-rw-rw-r--   0 stariki   (1000) stariki   (1000)       20 2023-04-29 09:02:16.000000 bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/top_level.txt
```

### Comparing `bosanski_kalkulator-0.1.1/LICENSE` & `bosanski_kalkulator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bosanski_kalkulator-0.1.1/PKG-INFO` & `bosanski_kalkulator-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosanski_kalkulator
-Version: 0.1.1
+Version: 0.1.2
 Summary: najbolji kalkulator
 Home-page: https://github.com/ona-li-toki-e-jan-Epiphany-tawa-mi/Bosanski-Kalkulator
 Download-URL: https://github.com/ona-li-toki-e-jan-Epiphany-tawa-mi/Bosanski-Kalkulator/releases
 Author: ona li toki e jan Epiphany tawa mi
 License: MIT
 Keywords: Bosanski Kalkulator,calculator,kalkulator,bosnian,bosnia,bosna,bosanski
 Platform: Windows
@@ -86,21 +86,24 @@
 
 Then the [main script](src/bosanski_kalkulator/main.py "main.py") can then be run using either of the following commands in the project directory:
 ```console
 python3 src/bosanski_kalkulator/main.py
 ./src/bosanski_kalkulator/main.py
 ```
 
-## Support
+## Credits
 
-If you like Bosanski Kalkulator and wish to support me, consider at one of the following link(s):
+The audio file [bosanska_artiljerija.mp3] was pulled from [Bosnian Folk Song - Bosanska Artiljerija](bosanska_artiljerija.mp3 "Bosnian Folk Song - Bosanska Artiljerija") on YouTube by [Folk Songs International,](https://www.youtube.com/@FolkSongsInternational "Folk Songs International's YouTube channel") make sure to check out their channel!
 
-https://github.com/sponsors/ona-li-toki-e-jan-Epiphany-tawa-mi
 # Changelog
 
+Added missing credits and removed obnoxious sponsor link 
+
+# 0.1.1
+
 - Fixed issue with dependencies not being automatically installed when installing.
 
 # 0.1.0
 
 - Initial release.
```

### Comparing `bosanski_kalkulator-0.1.1/setup.cfg` & `bosanski_kalkulator-0.1.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bosanski_kalkulator
-version = 0.1.1
+version = 0.1.2
 author = ona li toki e jan Epiphany tawa mi
 description = najbolji kalkulator
 long_description = file: README.md, CHANGELOG.md, LICENSE
 long_description_content_type = text/markdown
 keywords = Bosanski Kalkulator, calculator, kalkulator, bosnian, bosnia, bosna, bosanski
 license = MIT
 platforms = Windows, POSIX, MacOS
```

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/audio/bosanska_artiljerija.mp3` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/audio/bosanska_artiljerija.mp3`

 * *Files identical despite different names*

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/audio/pucnjava.mp3` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/audio/pucnjava.mp3`

 * *Files identical despite different names*

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/images/zastava_bosne_i_hercegovine.png` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/images/zastava_bosne_i_hercegovine.png`

 * *Files identical despite different names*

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator/main.py` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator/main.py`

 * *Files identical despite different names*

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/PKG-INFO` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosanski-kalkulator
-Version: 0.1.1
+Version: 0.1.2
 Summary: najbolji kalkulator
 Home-page: https://github.com/ona-li-toki-e-jan-Epiphany-tawa-mi/Bosanski-Kalkulator
 Download-URL: https://github.com/ona-li-toki-e-jan-Epiphany-tawa-mi/Bosanski-Kalkulator/releases
 Author: ona li toki e jan Epiphany tawa mi
 License: MIT
 Keywords: Bosanski Kalkulator,calculator,kalkulator,bosnian,bosnia,bosna,bosanski
 Platform: Windows
@@ -86,21 +86,24 @@
 
 Then the [main script](src/bosanski_kalkulator/main.py "main.py") can then be run using either of the following commands in the project directory:
 ```console
 python3 src/bosanski_kalkulator/main.py
 ./src/bosanski_kalkulator/main.py
 ```
 
-## Support
+## Credits
 
-If you like Bosanski Kalkulator and wish to support me, consider at one of the following link(s):
+The audio file [bosanska_artiljerija.mp3] was pulled from [Bosnian Folk Song - Bosanska Artiljerija](bosanska_artiljerija.mp3 "Bosnian Folk Song - Bosanska Artiljerija") on YouTube by [Folk Songs International,](https://www.youtube.com/@FolkSongsInternational "Folk Songs International's YouTube channel") make sure to check out their channel!
 
-https://github.com/sponsors/ona-li-toki-e-jan-Epiphany-tawa-mi
 # Changelog
 
+Added missing credits and removed obnoxious sponsor link 
+
+# 0.1.1
+
 - Fixed issue with dependencies not being automatically installed when installing.
 
 # 0.1.0
 
 - Initial release.
```

### Comparing `bosanski_kalkulator-0.1.1/src/bosanski_kalkulator.egg-info/SOURCES.txt` & `bosanski_kalkulator-0.1.2/src/bosanski_kalkulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


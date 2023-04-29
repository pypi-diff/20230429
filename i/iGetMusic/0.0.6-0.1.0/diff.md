# Comparing `tmp/iGetMusic-0.0.6.tar.gz` & `tmp/iGetMusic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iGetMusic-0.0.6.tar", last modified: Wed Dec 28 13:53:55 2022, max compression
+gzip compressed data, was "iGetMusic-0.1.0.tar", last modified: Sat Apr 29 14:54:37 2023, max compression
```

## Comparing `iGetMusic-0.0.6.tar` & `iGetMusic-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 13:53:55.067716 iGetMusic-0.0.6/
--rw-rw-rw-   0        0        0     1087 2022-12-23 21:25:13.000000 iGetMusic-0.0.6/LICENCE
--rw-rw-rw-   0        0        0     2915 2022-12-28 13:53:55.068714 iGetMusic-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2467 2022-12-28 13:52:06.000000 iGetMusic-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-28 13:53:55.059736 iGetMusic-0.0.6/iGetMusic/
--rw-rw-rw-   0        0        0      192 2022-12-27 19:50:59.000000 iGetMusic-0.0.6/iGetMusic/__init__.py
--rw-rw-rw-   0        0        0     5239 2022-12-28 13:50:21.000000 iGetMusic-0.0.6/iGetMusic/iGet.py
-drwxrwxrwx   0        0        0        0 2022-12-28 13:53:55.066719 iGetMusic-0.0.6/iGetMusic.egg-info/
--rw-rw-rw-   0        0        0     2915 2022-12-28 13:53:55.000000 iGetMusic-0.0.6/iGetMusic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2022-12-28 13:53:55.000000 iGetMusic-0.0.6/iGetMusic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 13:53:55.000000 iGetMusic-0.0.6/iGetMusic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-12-28 13:53:55.000000 iGetMusic-0.0.6/iGetMusic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2022-12-23 21:23:38.000000 iGetMusic-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      545 2022-12-28 13:53:55.069711 iGetMusic-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 14:54:37.755553 iGetMusic-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2022-12-23 21:25:13.000000 iGetMusic-0.1.0/LICENCE
+-rw-rw-rw-   0        0        0     2935 2023-04-29 14:54:37.755553 iGetMusic-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-01-01 11:39:54.000000 iGetMusic-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 14:54:37.744450 iGetMusic-0.1.0/iGetMusic/
+-rw-rw-rw-   0        0        0      192 2022-12-27 19:50:59.000000 iGetMusic-0.1.0/iGetMusic/__init__.py
+-rw-rw-rw-   0        0        0     5254 2023-04-29 14:34:44.000000 iGetMusic-0.1.0/iGetMusic/iGet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:54:37.753559 iGetMusic-0.1.0/iGetMusic.egg-info/
+-rw-rw-rw-   0        0        0     2935 2023-04-29 14:54:37.000000 iGetMusic-0.1.0/iGetMusic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-04-29 14:54:37.000000 iGetMusic-0.1.0/iGetMusic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:54:37.000000 iGetMusic-0.1.0/iGetMusic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 14:54:37.000000 iGetMusic-0.1.0/iGetMusic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2022-12-23 21:23:38.000000 iGetMusic-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      545 2023-04-29 14:54:37.756550 iGetMusic-0.1.0/setup.cfg
```

### Comparing `iGetMusic-0.0.6/LICENCE` & `iGetMusic-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `iGetMusic-0.0.6/PKG-INFO` & `iGetMusic-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iGetMusic
-Version: 0.0.6
+Version: 0.1.0
 Summary: Search for music with the iTunes API
 Home-page: https://github.com/Waradu/iGetMusic
 Author: Waradu
 Author-email: einfach_noan@outlook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Use `pip install iGetMusic` to install the package.<br>
 **After that install requests `pip install requests`**<br>
 Import package with `import iGetMusic as iGet`
 
 ### Get song by name:
 This returns a list containing all the songs as objects:
 ```py
-song = iGet.get(term=songName, country="GB", explicit=True)
+song = iGet.get(term=songName, limit=50, country="GB", explicit=True)
 ```
 Get song information:
 ```py
 song[x]
   .getName() #Returns song name
   .getArtistName() #Returns song author name
   .getImage() #Returns image URL
@@ -44,15 +44,15 @@
   .searchForSongName(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of songs based on song name as objects
   .searchForArtist(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of artists based on song author name as objects
 ```
 
 ### Get artist by name:
 This returns a list containing all the artists as objects:
 ```py
-artist = iGet.getArtist(term=artistName, country="GB", explicit=True)
+artist = iGet.getArtist(term=artistName, limit=50, country="GB", explicit=True)
 ```
 Get artist information:
 ```py
 artist[x]
   .getName() #Returns artist name
   .getArtistLinkUrl() #Returns artist link Url
   .getArtistID() #Returns artist id
```

### Comparing `iGetMusic-0.0.6/README.md` & `iGetMusic-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Use `pip install iGetMusic` to install the package.<br>
 **After that install requests `pip install requests`**<br>
 Import package with `import iGetMusic as iGet`
 
 ### Get song by name:
 This returns a list containing all the songs as objects:
 ```py
-song = iGet.get(term=songName, country="GB", explicit=True)
+song = iGet.get(term=songName, limit=50, country="GB", explicit=True)
 ```
 Get song information:
 ```py
 song[x]
   .getName() #Returns song name
   .getArtistName() #Returns song author name
   .getImage() #Returns image URL
@@ -30,15 +30,15 @@
   .searchForSongName(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of songs based on song name as objects
   .searchForArtist(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of artists based on song author name as objects
 ```
 
 ### Get artist by name:
 This returns a list containing all the artists as objects:
 ```py
-artist = iGet.getArtist(term=artistName, country="GB", explicit=True)
+artist = iGet.getArtist(term=artistName, limit=50, country="GB", explicit=True)
 ```
 Get artist information:
 ```py
 artist[x]
   .getName() #Returns artist name
   .getArtistLinkUrl() #Returns artist link Url
   .getArtistID() #Returns artist id
```

### Comparing `iGetMusic-0.0.6/iGetMusic/iGet.py` & `iGetMusic-0.1.0/iGetMusic/iGet.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 
     for item in data:
         songList.append(song(item))
 
     return songList
 
 
-def getArtist(term, country="GB", explicit=True):
+def getArtist(term, country="GB", limit=1, explicit=True):
 
-    apiUrl = f"{itunes}term={term}&entity=allArtist&country={country}&limit=1&explicit={'Yes' if explicit else 'No'}"
+    apiUrl = f"{itunes}term={term}&entity=allArtist&country={country}&limit={limit}&explicit={'Yes' if explicit else 'No'}"
     r = requests.get(apiUrl)
     data = r.json()
 
     data = data["results"]
 
     songList = []
```

### Comparing `iGetMusic-0.0.6/iGetMusic.egg-info/PKG-INFO` & `iGetMusic-0.1.0/iGetMusic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iGetMusic
-Version: 0.0.6
+Version: 0.1.0
 Summary: Search for music with the iTunes API
 Home-page: https://github.com/Waradu/iGetMusic
 Author: Waradu
 Author-email: einfach_noan@outlook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Use `pip install iGetMusic` to install the package.<br>
 **After that install requests `pip install requests`**<br>
 Import package with `import iGetMusic as iGet`
 
 ### Get song by name:
 This returns a list containing all the songs as objects:
 ```py
-song = iGet.get(term=songName, country="GB", explicit=True)
+song = iGet.get(term=songName, limit=50, country="GB", explicit=True)
 ```
 Get song information:
 ```py
 song[x]
   .getName() #Returns song name
   .getArtistName() #Returns song author name
   .getImage() #Returns image URL
@@ -44,15 +44,15 @@
   .searchForSongName(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of songs based on song name as objects
   .searchForArtist(country="GB", limit=50, explicit=True) #Returns list with "limit" amount of artists based on song author name as objects
 ```
 
 ### Get artist by name:
 This returns a list containing all the artists as objects:
 ```py
-artist = iGet.getArtist(term=artistName, country="GB", explicit=True)
+artist = iGet.getArtist(term=artistName, limit=50, country="GB", explicit=True)
 ```
 Get artist information:
 ```py
 artist[x]
   .getName() #Returns artist name
   .getArtistLinkUrl() #Returns artist link Url
   .getArtistID() #Returns artist id
```

### Comparing `iGetMusic-0.0.6/setup.cfg` & `iGetMusic-0.1.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 4765 744d 7573 6963 0d0a 7665   = iGetMusic..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 360d 0a61  rsion = 0.0.6..a
+00000020: 7273 696f 6e20 3d20 302e 312e 300d 0a61  rsion = 0.1.0..a
 00000030: 7574 686f 7220 3d20 5761 7261 6475 0d0a  uthor = Waradu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2065  author_email = e
 00000050: 696e 6661 6368 5f6e 6f61 6e40 6f75 746c  infach_noan@outl
 00000060: 6f6f 6b2e 6465 0d0a 6465 7363 7269 7074  ook.de..descript
 00000070: 696f 6e20 3d20 5365 6172 6368 2066 6f72  ion = Search for
 00000080: 206d 7573 6963 2077 6974 6820 7468 6520   music with the 
 00000090: 6954 756e 6573 2041 5049 0d0a 6c6f 6e67  iTunes API..long
```


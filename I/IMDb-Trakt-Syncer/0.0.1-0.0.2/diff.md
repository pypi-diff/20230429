# Comparing `tmp/IMDb-Trakt-Syncer-0.0.1.tar.gz` & `tmp/IMDb-Trakt-Syncer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDb-Trakt-Syncer-0.0.1.tar", last modified: Sat Apr 29 01:27:12 2023, max compression
+gzip compressed data, was "IMDb-Trakt-Syncer-0.0.2.tar", last modified: Sat Apr 29 01:34:51 2023, max compression
```

## Comparing `IMDb-Trakt-Syncer-0.0.1.tar` & `IMDb-Trakt-Syncer-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 01:27:12.818728 IMDb-Trakt-Syncer-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-29 01:27:12.798457 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     6283 2023-04-29 00:08:08.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-04-28 21:58:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-04-28 23:59:44.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3577 2023-04-29 00:02:08.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1731 2023-04-28 21:49:21.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1596 2023-04-28 21:38:36.000000 IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-04-29 01:27:12.816229 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/
--rw-rw-rw-   0        0        0     4799 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 01:27:12.000000 IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDb-Trakt-Syncer-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4799 2023-04-29 01:27:12.818228 IMDb-Trakt-Syncer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4233 2023-04-29 01:25:00.000000 IMDb-Trakt-Syncer-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 01:27:12.819228 IMDb-Trakt-Syncer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1231 2023-04-29 01:26:56.000000 IMDb-Trakt-Syncer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 01:34:51.422709 IMDb-Trakt-Syncer-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-29 01:34:51.398500 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     6283 2023-04-29 00:08:08.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-04-28 21:58:12.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-04-28 23:59:44.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3577 2023-04-29 00:02:08.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1731 2023-04-28 21:49:21.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1596 2023-04-28 21:38:36.000000 IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-04-29 01:34:51.420201 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/
+-rw-rw-rw-   0        0        0     4799 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 01:34:51.000000 IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDb-Trakt-Syncer-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4799 2023-04-29 01:34:51.421709 IMDb-Trakt-Syncer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4233 2023-04-29 01:25:00.000000 IMDb-Trakt-Syncer-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 01:34:51.422709 IMDb-Trakt-Syncer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2023-04-29 01:34:31.000000 IMDb-Trakt-Syncer-0.0.2/setup.py
```

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/authTrakt.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/checkChromedriver.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/imdbRatings.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/traktRatings.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDbTraktSyncer/verifyCredentials.py` & `IMDb-Trakt-Syncer-0.0.2/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/IMDb_Trakt_Syncer.egg-info/PKG-INFO` & `IMDb-Trakt-Syncer-0.0.2/IMDb_Trakt_Syncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDb-Trakt-Syncer
-Version: 0.0.1
+Version: 0.0.2
 Summary: This script will sync user ratings both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDb-Trakt-Syncer-0.0.1/LICENSE` & `IMDb-Trakt-Syncer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/PKG-INFO` & `IMDb-Trakt-Syncer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDb-Trakt-Syncer
-Version: 0.0.1
+Version: 0.0.2
 Summary: This script will sync user ratings both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDb-Trakt-Syncer-0.0.1/README.md` & `IMDb-Trakt-Syncer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `IMDb-Trakt-Syncer-0.0.1/setup.py` & `IMDb-Trakt-Syncer-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'This script will sync user ratings both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDb-Trakt-Syncer",
     version=VERSION,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/RileyXX/IMDb-Trakt-Syncer",
     packages=find_packages(),
-    install_requires=['plexapi'],
+    install_requires=['requests', 'feedparser', 'subprocess', 'selenium'],
     keywords=['python', 'video', 'trakt', 'imdb', 'ratings', 'sync', 'movies', 'tv shows'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```


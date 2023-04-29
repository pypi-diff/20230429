# Comparing `tmp/relic_engine-0.2.5.tar.gz` & `tmp/relic_engine-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relic_engine-0.2.5.tar", last modified: Fri Mar 10 03:32:42 2023, max compression
+gzip compressed data, was "relic_engine-0.2.6.tar", last modified: Wed Apr 12 00:53:22 2023, max compression
```

## Comparing `relic_engine-0.2.5.tar` & `relic_engine-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 03:32:42.292736 relic_engine-0.2.5/
--rw-rw-rw-   0        0        0      454 2023-03-10 03:32:42.291736 relic_engine-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-10 03:32:42.288899 relic_engine-0.2.5/relic_engine/
--rw-rw-rw-   0        0        0     5835 2023-03-10 03:32:27.000000 relic_engine-0.2.5/relic_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 03:32:42.291736 relic_engine-0.2.5/relic_engine.egg-info/
--rw-rw-rw-   0        0        0      454 2023-03-10 03:32:42.000000 relic_engine-0.2.5/relic_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-03-10 03:32:42.000000 relic_engine-0.2.5/relic_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 03:32:42.000000 relic_engine-0.2.5/relic_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-10 03:32:42.000000 relic_engine-0.2.5/relic_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-10 03:32:42.000000 relic_engine-0.2.5/relic_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 03:32:42.292736 relic_engine-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-03-10 03:32:36.000000 relic_engine-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:53:22.280034 relic_engine-0.2.6/
+-rw-rw-rw-   0        0        0      454 2023-04-12 00:53:22.280034 relic_engine-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 00:53:22.277034 relic_engine-0.2.6/relic_engine/
+-rw-rw-rw-   0        0        0     5832 2023-04-12 00:52:12.000000 relic_engine-0.2.6/relic_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:53:22.279032 relic_engine-0.2.6/relic_engine.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-12 00:53:22.000000 relic_engine-0.2.6/relic_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-12 00:53:22.000000 relic_engine-0.2.6/relic_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:53:22.000000 relic_engine-0.2.6/relic_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 00:53:22.000000 relic_engine-0.2.6/relic_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 00:53:22.000000 relic_engine-0.2.6/relic_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 00:53:22.280034 relic_engine-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-04-12 00:52:21.000000 relic_engine-0.2.6/setup.py
```

### Comparing `relic_engine-0.2.5/relic_engine/__init__.py` & `relic_engine-0.2.6/relic_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def __decode_and_decompress(url):
     file = requests.get(url).content
     file = gzip.decompress(file)
     return json.loads(file.decode("utf-8"))
 
 
 def __get_index_file():
-    index = __decode_and_decompress("http://107.175.127.29/index/index.json.gz")
+    index = __decode_and_decompress("https://relics.run/index/index.json.gz")
 
     return index
 
 
 __index = __get_index_file()
 __relic_dict = __index['relics']
 __price_dict = __index['prices']
```

### Comparing `relic_engine-0.2.5/setup.py` & `relic_engine-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.5' 
+VERSION = '0.2.6' 
 DESCRIPTION = 'Engine for generating dictionaries of relics and prime sets.'
 LONG_DESCRIPTION = 'Engine for generating dictionaries of relics and prime sets using Digital Extreme\'s PC drops website and warframe.market price data.'
 
 setup(
         name="relic_engine", 
         version=VERSION,
         author="Jacob McBride",
```


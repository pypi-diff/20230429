# Comparing `tmp/nsepython-1.4.tar.gz` & `tmp/nsepython-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepython-1.4.tar", last modified: Wed Apr 26 21:06:55 2023, max compression
+gzip compressed data, was "nsepython-1.5.tar", last modified: Sat Apr 29 05:39:51 2023, max compression
```

## Comparing `nsepython-1.4.tar` & `nsepython-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:55.061635 nsepython-1.4/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1.4/LICENSE
--rw-rw-rw-   0        0        0     2374 2023-04-26 21:06:55.060612 nsepython-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:55.037698 nsepython-1.4/nsepython/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1.4/nsepython/__init__.py
--rw-rw-rw-   0        0        0    35819 2023-04-26 21:06:08.000000 nsepython-1.4/nsepython/rahu.py
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:55.059084 nsepython-1.4/nsepython.egg-info/
--rw-rw-rw-   0        0        0     2374 2023-04-26 21:06:54.000000 nsepython-1.4/nsepython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-26 21:06:54.000000 nsepython-1.4/nsepython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 21:06:54.000000 nsepython-1.4/nsepython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 21:06:54.000000 nsepython-1.4/nsepython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 21:06:54.000000 nsepython-1.4/nsepython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 21:06:55.062148 nsepython-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-04-26 21:06:21.000000 nsepython-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:39:51.678375 nsepython-1.5/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1.5/LICENSE
+-rw-rw-rw-   0        0        0     2374 2023-04-29 05:39:51.648114 nsepython-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 05:39:51.512715 nsepython-1.5/nsepython/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1.5/nsepython/__init__.py
+-rw-rw-rw-   0        0        0    35828 2023-04-29 05:35:43.000000 nsepython-1.5/nsepython/rahu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:39:51.643988 nsepython-1.5/nsepython.egg-info/
+-rw-rw-rw-   0        0        0     2374 2023-04-29 05:39:48.000000 nsepython-1.5/nsepython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-29 05:39:48.000000 nsepython-1.5/nsepython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 05:39:48.000000 nsepython-1.5/nsepython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-29 05:39:48.000000 nsepython-1.5/nsepython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 05:39:48.000000 nsepython-1.5/nsepython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 05:39:51.678891 nsepython-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-04-29 05:37:32.000000 nsepython-1.5/setup.py
```

### Comparing `nsepython-1.4/LICENSE` & `nsepython-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepython-1.4/PKG-INFO` & `nsepython-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1.4
+Version: 1.5
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nsepython Version: 1.4 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.5 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1.4/README.md` & `nsepython-1.5/README.md`

 * *Files identical despite different names*

### Comparing `nsepython-1.4/nsepython/rahu.py` & `nsepython-1.5/nsepython/rahu.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 import pandas as pd
 import json
 import random
 import datetime,time
 import logging
 import re
-import urllib.parse 
+import urllib.parse
 
 mode ='local'
 
 if(mode=='local'):
     def nsefetch(payload):
         output = requests.get(payload,headers=headers).json()
         return output
@@ -575,19 +575,20 @@
     return payload
 
 def derivative_history_virgin(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice="",optionType=""):
 
     instrumentType = instrumentType.lower()
 
     if(instrumentType=="options"):
-        if("NIFTY" in symbol): instrumentType="FUTSTK"
         instrumentType="OPTSTK"
-    if(instrumentType=="futures"):
         if("NIFTY" in symbol): instrumentType="OPTIDX"
-        instrumentType="FUTIDX"
+        
+    if(instrumentType=="futures"):
+        instrumentType="FUTSTK"
+        if("NIFTY" in symbol): instrumentType="FUTIDX"
 
     if(((instrumentType=="OPTIDX")or (instrumentType=="OPTSTK")) and (expiry_date!="")):
         strikePrice = "%.2f" % strikePrice
         strikePrice = str(strikePrice)
 
     nsefetch_url = "https://www.nseindia.com/api/historical/fo/derivatives?&from="+str(start_date)+"&to="+str(end_date)+"&optionType="+optionType+"&strikePrice="+strikePrice+"&expiryDate="+expiry_date+"&instrumentType="+instrumentType+"&symbol="+symbol+""
     payload = nsefetch(nsefetch_url)
```

### Comparing `nsepython-1.4/nsepython.egg-info/PKG-INFO` & `nsepython-1.5/nsepython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 1.4
+Version: 1.5
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nsepython Version: 1.4 Summary: Python library for
+Metadata-Version: 2.1 Name: nsepython Version: 1.5 Summary: Python library for
 NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepython-1.4/setup.py` & `nsepython-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepython',
     packages=setuptools.find_packages(),
-    version = '1.4',
+    version = '1.5',
     include_package_data=True,
     description = 'Python library for NSE India APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Aeron7',
     author_email = 'dexter@unofficed.com',
     url = 'https://github.com/aeron7/nsepython',
     install_requires=['requests', 'pandas','scipy'],
```


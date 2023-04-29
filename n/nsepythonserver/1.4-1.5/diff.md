# Comparing `tmp/nsepythonserver-1.4.tar.gz` & `tmp/nsepythonserver-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepythonserver-1.4.tar", last modified: Wed Apr 26 21:06:27 2023, max compression
+gzip compressed data, was "nsepythonserver-1.5.tar", last modified: Sat Apr 29 05:42:23 2023, max compression
```

## Comparing `nsepythonserver-1.4.tar` & `nsepythonserver-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:27.144002 nsepythonserver-1.4/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepythonserver-1.4/LICENSE
--rw-rw-rw-   0        0        0     2380 2023-04-26 21:06:27.142470 nsepythonserver-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepythonserver-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:27.117987 nsepythonserver-1.4/nsepythonserver/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepythonserver-1.4/nsepythonserver/__init__.py
--rw-rw-rw-   0        0        0    36431 2023-04-26 21:06:09.000000 nsepythonserver-1.4/nsepythonserver/rahu.py
-drwxrwxrwx   0        0        0        0 2023-04-26 21:06:27.140421 nsepythonserver-1.4/nsepythonserver.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-04-26 21:06:26.000000 nsepythonserver-1.4/nsepythonserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-26 21:06:26.000000 nsepythonserver-1.4/nsepythonserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 21:06:26.000000 nsepythonserver-1.4/nsepythonserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 21:06:26.000000 nsepythonserver-1.4/nsepythonserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 21:06:26.000000 nsepythonserver-1.4/nsepythonserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 21:06:27.144510 nsepythonserver-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-04-26 21:06:17.000000 nsepythonserver-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:42:23.453415 nsepythonserver-1.5/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepythonserver-1.5/LICENSE
+-rw-rw-rw-   0        0        0     2380 2023-04-29 05:42:23.450804 nsepythonserver-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepythonserver-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 05:42:23.355408 nsepythonserver-1.5/nsepythonserver/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepythonserver-1.5/nsepythonserver/__init__.py
+-rw-rw-rw-   0        0        0    36441 2023-04-29 05:36:16.000000 nsepythonserver-1.5/nsepythonserver/rahu.py
+drwxrwxrwx   0        0        0        0 2023-04-29 05:42:23.447192 nsepythonserver-1.5/nsepythonserver.egg-info/
+-rw-rw-rw-   0        0        0     2380 2023-04-29 05:42:22.000000 nsepythonserver-1.5/nsepythonserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-29 05:42:23.000000 nsepythonserver-1.5/nsepythonserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 05:42:22.000000 nsepythonserver-1.5/nsepythonserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-29 05:42:22.000000 nsepythonserver-1.5/nsepythonserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 05:42:22.000000 nsepythonserver-1.5/nsepythonserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 05:42:23.453934 nsepythonserver-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-29 05:37:24.000000 nsepythonserver-1.5/setup.py
```

### Comparing `nsepythonserver-1.4/LICENSE` & `nsepythonserver-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepythonserver-1.4/PKG-INFO` & `nsepythonserver-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepythonserver
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
-Metadata-Version: 2.1 Name: nsepythonserver Version: 1.4 Summary: Python
+Metadata-Version: 2.1 Name: nsepythonserver Version: 1.5 Summary: Python
 library for NSE India APIs Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepythonserver-1.4/README.md` & `nsepythonserver-1.5/README.md`

 * *Files identical despite different names*

### Comparing `nsepythonserver-1.4/nsepythonserver/rahu.py` & `nsepythonserver-1.5/nsepythonserver/rahu.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,19 +589,20 @@
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

### Comparing `nsepythonserver-1.4/nsepythonserver.egg-info/PKG-INFO` & `nsepythonserver-1.5/nsepythonserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepythonserver
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
-Metadata-Version: 2.1 Name: nsepythonserver Version: 1.4 Summary: Python
+Metadata-Version: 2.1 Name: nsepythonserver Version: 1.5 Summary: Python
 library for NSE India APIs Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7 Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
```

### Comparing `nsepythonserver-1.4/setup.py` & `nsepythonserver-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepythonserver',
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


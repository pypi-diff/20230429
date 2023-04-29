# Comparing `tmp/GoogleNews-1.6.7.tar.gz` & `tmp/GoogleNews-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleNews-1.6.7.tar", last modified: Fri Mar 24 23:38:02 2023, max compression
+gzip compressed data, was "GoogleNews-1.6.8.tar", last modified: Sat Apr 29 05:06:58 2023, max compression
```

## Comparing `GoogleNews-1.6.7.tar` & `GoogleNews-1.6.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 23:38:02.487055 GoogleNews-1.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 23:38:02.483055 GoogleNews-1.6.7/GoogleNews/
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/GoogleNews/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 23:38:02.483055 GoogleNews-1.6.7/GoogleNews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-24 23:38:02.000000 GoogleNews-1.6.7/GoogleNews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 23:38:02.000000 GoogleNews-1.6.7/GoogleNews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 23:38:02.000000 GoogleNews-1.6.7/GoogleNews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-24 23:38:02.000000 GoogleNews-1.6.7/GoogleNews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 23:38:02.000000 GoogleNews-1.6.7/GoogleNews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-24 23:38:02.487055 GoogleNews-1.6.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 23:38:02.487055 GoogleNews-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 23:38:02.483055 GoogleNews-1.6.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-24 23:37:49.000000 GoogleNews-1.6.7/test/test_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:06:58.255725 GoogleNews-1.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:06:58.251725 GoogleNews-1.6.8/GoogleNews/
+-rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/GoogleNews/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:06:58.251725 GoogleNews-1.6.8/GoogleNews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-29 05:06:58.000000 GoogleNews-1.6.8/GoogleNews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 05:06:58.000000 GoogleNews-1.6.8/GoogleNews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:06:58.000000 GoogleNews-1.6.8/GoogleNews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-29 05:06:58.000000 GoogleNews-1.6.8/GoogleNews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 05:06:58.000000 GoogleNews-1.6.8/GoogleNews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-29 05:06:58.255725 GoogleNews-1.6.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:06:58.255725 GoogleNews-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:06:58.255725 GoogleNews-1.6.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-29 05:06:44.000000 GoogleNews-1.6.8/test/test_sort.py
```

### Comparing `GoogleNews-1.6.7/GoogleNews/__init__.py` & `GoogleNews-1.6.8/GoogleNews/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         else:
             self.headers = {'User-Agent': self.user_agent}
         self.__period = period
         self.__start = start
         self.__end = end
         self.__encode = encode
         self.__exception = False
-        self.__version = '1.6.7'
+        self.__version = '1.6.8'
 
     def getVersion(self):
         return self.__version
     
     def enableException(self, enable=True):
         self.__exception = enable
 
@@ -121,15 +121,15 @@
 
     def search(self, key):
         """
         Searches for a term in google.com in the news section and retrieves the first page into __results.
         Parameters:
         key = the search term
         """
-        self.__key = "+".join(key.split(" "))
+        self.__key = key
         if self.__encode != "":
             self.__key = urllib.request.quote(self.__key.encode(self.__encode))
         self.get_page()
 
     def build_response(self):
         self.req = urllib.request.Request(self.url.replace("search?","search?hl="+self.__lang+"&gl="+self.__lang+"&"), headers=self.headers)
         self.response = urllib.request.urlopen(self.req)
@@ -260,16 +260,15 @@
     def getpage(self, page=1):
         """Don't remove this, will affect old version user when upgrade"""
         self.get_page(page)
 
     def get_news(self, key="",deamplify=False):
         if key != '':
             if self.__period != "":
-                key += f"+when:{self.__period}"
-            key = "+".join(key.split(" "))
+                key += f" when:{self.__period}"
         else:
             if self.__period != "":
                 key += f"when:{self.__period}"
         key = urllib.request.quote(key.encode(self.__encode))
         self.url = 'https://news.google.com/search?q={}&hl={}'.format(key,self.__lang.lower())
 
         try:
@@ -383,8 +382,8 @@
         """Returns only the __links of the __results."""
         return self.__links
 
     def clear(self):
         self.__texts = []
         self.__links = []
         self.__results = []
-        self.__totalcount = 0
+        self.__totalcount = 0
```

### Comparing `GoogleNews-1.6.7/GoogleNews.egg-info/PKG-INFO` & `GoogleNews-1.6.8/GoogleNews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNews
-Version: 1.6.7
+Version: 1.6.8
 Summary: Google News search for Python
 Home-page: https://github.com/Iceloof/GoogleNews
 Author: Hurin Hu
 Author-email: hurin@live.ca
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GoogleNews-1.6.7/LICENSE` & `GoogleNews-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleNews-1.6.7/PKG-INFO` & `GoogleNews-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNews
-Version: 1.6.7
+Version: 1.6.8
 Summary: Google News search for Python
 Home-page: https://github.com/Iceloof/GoogleNews
 Author: Hurin Hu
 Author-email: hurin@live.ca
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GoogleNews-1.6.7/README.md` & `GoogleNews-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `GoogleNews-1.6.7/setup.py` & `GoogleNews-1.6.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GoogleNews",
-    version="1.6.7",
+    version="1.6.8",
     author="Hurin Hu",
     author_email="hurin@live.ca",
     description="Google News search for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Iceloof/GoogleNews",
     packages=setuptools.find_packages(),
```

### Comparing `GoogleNews-1.6.7/test/test_search.py` & `GoogleNews-1.6.8/test/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     self.assertEqual(length, 10)
     print('Result length at two pages is correct')
 
 class TestStringMethods(unittest.TestCase):
 
   def testVersion(self):
     googlenews = GoogleNews()
-    version = '1.6.7'
+    version = '1.6.8'
     self.assertIn(version, googlenews.getVersion())
     print('Latest version matched')
     
   def testResultContainsKeyword(self):
     googlenews = GoogleNews()
     googlenews.search(keyword)
     result = googlenews.result()[0]
```

### Comparing `GoogleNews-1.6.7/test/test_sort.py` & `GoogleNews-1.6.8/test/test_sort.py`

 * *Files identical despite different names*


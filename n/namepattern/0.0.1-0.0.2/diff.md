# Comparing `tmp/namepattern-0.0.1.tar.gz` & `tmp/namepattern-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namepattern-0.0.1.tar", last modified: Wed Apr 12 21:24:44 2023, max compression
+gzip compressed data, was "namepattern-0.0.2.tar", last modified: Sat Apr 29 19:05:55 2023, max compression
```

## Comparing `namepattern-0.0.1.tar` & `namepattern-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-12 21:24:44.068755 namepattern-0.0.1/
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)     1076 2023-04-12 21:00:56.000000 namepattern-0.0.1/LICENSE
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      724 2023-04-12 21:24:44.068425 namepattern-0.0.1/PKG-INFO
-drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-12 21:24:44.064580 namepattern-0.0.1/namepattern/
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)    10848 2023-04-12 21:24:15.000000 namepattern-0.0.1/namepattern/__init__.py
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)    10848 2023-04-12 20:51:24.000000 namepattern-0.0.1/namepattern/namepattern.py
-drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-12 21:24:44.066753 namepattern-0.0.1/namepattern.egg-info/
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      724 2023-04-12 21:24:44.000000 namepattern-0.0.1/namepattern.egg-info/PKG-INFO
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      207 2023-04-12 21:24:44.000000 namepattern-0.0.1/namepattern.egg-info/SOURCES.txt
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        1 2023-04-12 21:24:44.000000 namepattern-0.0.1/namepattern.egg-info/dependency_links.txt
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)       12 2023-04-12 21:24:44.000000 namepattern-0.0.1/namepattern.egg-info/top_level.txt
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)       38 2023-04-12 21:24:44.068883 namepattern-0.0.1/setup.cfg
--rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      912 2023-04-12 21:14:49.000000 namepattern-0.0.1/setup.py
+drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-29 19:05:55.029534 namepattern-0.0.2/
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)     1076 2023-04-12 21:00:56.000000 namepattern-0.0.2/LICENSE
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      729 2023-04-29 19:05:55.029185 namepattern-0.0.2/PKG-INFO
+drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-29 19:05:55.024627 namepattern-0.0.2/namepattern/
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)    11021 2023-04-29 18:10:54.000000 namepattern-0.0.2/namepattern/__init__.py
+drwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        0 2023-04-29 19:05:55.028187 namepattern-0.0.2/namepattern.egg-info/
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      729 2023-04-29 19:05:54.000000 namepattern-0.0.2/namepattern.egg-info/PKG-INFO
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      180 2023-04-29 19:05:54.000000 namepattern-0.0.2/namepattern.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)        1 2023-04-29 19:05:54.000000 namepattern-0.0.2/namepattern.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)       12 2023-04-29 19:05:54.000000 namepattern-0.0.2/namepattern.egg-info/top_level.txt
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)       38 2023-04-29 19:05:55.029661 namepattern-0.0.2/setup.cfg
+-rwxrwxrwx   0 rancho2002  (1000) rancho2002  (1000)      917 2023-04-29 18:16:58.000000 namepattern-0.0.2/setup.py
```

### Comparing `namepattern-0.0.1/LICENSE` & `namepattern-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `namepattern-0.0.1/PKG-INFO` & `namepattern-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namepattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: Printing name pattern with python
 Home-page: UNKNOWN
 Author: Arijit Ghosh
 Author-email: subhasghosh196@gmail.com
 License: UNKNOWN
 Keywords: python,namepattern,pattern
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern.
+A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern. Use
```

### Comparing `namepattern-0.0.1/namepattern/__init__.py` & `namepattern-0.0.2/namepattern/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,21 +286,25 @@
             else:
                 print(len(point)*" ", end="")
         print()
 
 
 
 class Namepattern:
+
+    def __str__(self) -> str:
+        return "\n\n****This object now can print any pattern you give as argument. Use displayName() function to print the pattern in terminal.****\n\n"
+
     def __init__(self,pattern: str,design:str="^^",n:int=5) -> None:
         self.pattern=pattern
         self.design=design
         self.n=n
 
     def displayName(self) -> None:
-            '''This function will print the any name as pattern'''
+            '''\n\n****This function takes no argument and returns None. So, function call is enough to see the pattern.****\n\n'''
             # create a docstring
             pattern=self.pattern.upper()
             design=self.design
             n=self.n
             for i in pattern:
                 if i == "A":
                     A(design, n)
@@ -351,15 +355,13 @@
                 elif i == "X":
                     X(design, n)
                 elif i == "Y":
                     Y(design, n)
                 elif i == "Z":
                     Z(design, n)
                 elif i==" ":
-                    print("\n")
+                    print()
                 else:
                     print("Invalid character found at index", i, ". Program Terminated.")
                     exit(0)
-                #space between letters
-                print("\n")
+                print()
 
-# displayName("Arij32it ghosh")
```

### Comparing `namepattern-0.0.1/namepattern.egg-info/PKG-INFO` & `namepattern-0.0.2/namepattern.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namepattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: Printing name pattern with python
 Home-page: UNKNOWN
 Author: Arijit Ghosh
 Author-email: subhasghosh196@gmail.com
 License: UNKNOWN
 Keywords: python,namepattern,pattern
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern.
+A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern. Use
```

### Comparing `namepattern-0.0.1/setup.py` & `namepattern-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Printing name pattern with python'
-LONG_DESCRIPTION = 'A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern.'
+LONG_DESCRIPTION = 'A package that prints name pattern with python takes input, design style(pattern type), and length from user and prints the pattern. Use '
 
 # Setting up
 setup(
     name="namepattern",
     version=VERSION,
     author="Arijit Ghosh",
     author_email="subhasghosh196@gmail.com",
```


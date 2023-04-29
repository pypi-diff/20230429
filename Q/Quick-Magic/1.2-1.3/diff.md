# Comparing `tmp/Quick_Magic-1.2.tar.gz` & `tmp/Quick_Magic-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quick_Magic-1.2.tar", last modified: Sat Apr 29 16:29:25 2023, max compression
+gzip compressed data, was "Quick_Magic-1.3.tar", last modified: Sat Apr 29 18:16:38 2023, max compression
```

## Comparing `Quick_Magic-1.2.tar` & `Quick_Magic-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.672764 Quick_Magic-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 16:29:25.672764 Quick_Magic-1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.668764 Quick_Magic-1.2/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/update_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.672764 Quick_Magic-1.2/Quick_Magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 16:29:15.000000 Quick_Magic-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:29:25.672764 Quick_Magic-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 16:29:15.000000 Quick_Magic-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:16:38.965930 Quick_Magic-1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/update_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/Quick_Magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 18:16:24.000000 Quick_Magic-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:16:38.965930 Quick_Magic-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 18:16:24.000000 Quick_Magic-1.3/setup.py
```

### Comparing `Quick_Magic-1.2/PKG-INFO` & `Quick_Magic-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick_Magic
-Version: 1.2
+Version: 1.3
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.2/Quick_Magic/__init__.py` & `Quick_Magic-1.3/Quick_Magic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1"
+__version__ = "1.3"
 from . import check, update_list, commands, features
 import os, re
 
 check.check_os()
 # Checking if required files exists or not
 check.check_json()
 check.app_names()
@@ -120,15 +120,15 @@
                 j = i.strip()
                 if j != "":
                     features.open_things(j, output=output, match_closest=match_closest)
         else:
            features.open_things(val, output=output, match_closest=match_closest)
 
 # Close any application by just its name :)
-def close(self, output=True, match_closest=False):
+def close(self, output=True, match_closest=False, throw_error=False):
     '''
     #### `close` is the function which is used to close applications.
     Examples:
     1: close("whatsapp")
     2: close("whatsapp, telegram")
     3: close("calcu", match_closest=True)
     4: close("whatsapp, telegram", output=False)
@@ -142,11 +142,11 @@
     inp = (self).lower()
     val=(re.compile(r'[^a-zA-Z-^0-9?,>&+.]').sub(" ",inp)).strip()
     if "," in val:
         splited = val.split(",")
         for i in splited:
             j = i.strip()
             if j != "":
-                features.close_things(j, output=output, match_closest=match_closest)
+                features.close_things(j, output=output, match_closest=match_closest, throw_error=throw_error)
     else:
-        features.close_things(val, output=output, match_closest=match_closest)
+        features.close_things(val, output=output, match_closest=match_closest, throw_error=throw_error)
```

### Comparing `Quick_Magic-1.2/Quick_Magic/check.py` & `Quick_Magic-1.3/Quick_Magic/check.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.2/Quick_Magic/commands.py` & `Quick_Magic-1.3/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.2/Quick_Magic/features.py` & `Quick_Magic-1.3/Quick_Magic/features.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, json, sys, psutil, subprocess, difflib, inspect
+import os, json, sys, psutil, subprocess, difflib, inspect, win32gui, win32con
 
 # Defining a custom error message called AppNotFound
 class AppNotFound(Exception):
     def __init__(self, app_name):
         self.app_name = app_name
     
     def __str__(self):
@@ -46,15 +46,18 @@
             if output:
                 print("OPENING "+self.upper())
         except:
             result = difflib.get_close_matches(self,keys, n=1, cutoff=0.6)
             app_name = ' '.join(result).strip()
             if result:
                 if output:
+                    print()
                     print("Closest match to "+self.upper()+" : "+str(result))
+                    print(f'Try : [open("{self}", match_closest=True)]')
+                    print()
                 if match_closest:
                     dir01 = data1[app_name]
                     os.system("explorer shell:appsFolder\\"+dir01)
                     # print("explorer shell:appsFolder\\"+app_name)
                     if output:
                         print("OPENING "+app_name.upper())
             else:
@@ -62,20 +65,41 @@
                     if throw_error:
                         # Throwing an error if throw_error is true
                         raise ValueError(f"{self.upper()} NOT FOUND... TYPE (LS) for list of applications.")
                     else:
                         print(f"{self.upper()} NOT FOUND... TYPE (LS) for list of applications.")
             pass
 
+# EXCEPTION FOR CLOSING FILE EXPLORER
+def close_explorer(output: bool, throw_error: bool, app_name: str):
+    handles = []
+    win32gui.EnumWindows(lambda hwnd, param: param.append(hwnd) if win32gui.GetClassName(hwnd) == 'CabinetWClass' else None, handles)
+    # close all File Explorer windows
+    for handle in handles:
+        win32gui.PostMessage(handle, win32con.WM_CLOSE, 0, 0)
+    if not handles:
+        if output:
+            print((app_name.replace(".exe","")).upper() +" is not running")
+    else:
+        if output:
+            print("CLOSING "+(app_name.replace(".exe","")).upper())
+    if throw_error:
+        app_name = (app_name).upper()
+        raise AppNotFound(app_name)
+
 # CLOSE SEVERAL THINGS :)
 def close_things(self, output=True, match_closest=False, throw_error=False):
     if not self.endswith(".exe"):
         self = (self+".exe")
+    explorer_list = ["file explorer", "explorer"]
     flag = False
     if not match_closest:
+        if (self.replace(".exe", "").strip()) in explorer_list:
+            close_explorer(output=output, throw_error=throw_error, app_name=(self.replace(".exe","")))
+            return
         for pid in psutil.pids():
             try:
                 process = psutil.Process(pid)
                 if process.name().lower() == self:
                     process.kill()
                     if not flag and output:
                         print("CLOSING "+(self.replace(".exe","")).upper())
@@ -94,14 +118,19 @@
                 process = psutil.Process(pid)
                 app_jug.append((process.name()))
             except: pass
         result = difflib.get_close_matches(self,app_jug, n=1, cutoff=0.6)
         app_name = ' '.join(result).strip()
         # print(app_jug)
         # print(app_name)
+        ## EXCEPTION FOR CLOSING FILE EXPLORER
+        if (app_name.replace(".exe", "").strip()) in explorer_list:
+            # print("yes")
+            close_explorer(output=output, throw_error=throw_error, app_name=app_name)
+            return
         command = ['taskkill', '/f', '/im',app_name]
         # print(command)
         with open('NUL', 'w') as null:
             process = subprocess.Popen(command, stdout=null, stderr=null)
             process.wait()
             if process.returncode == 0:
                 if output:
```

### Comparing `Quick_Magic-1.2/Quick_Magic/update_list.py` & `Quick_Magic-1.3/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.2/Quick_Magic.egg-info/PKG-INFO` & `Quick_Magic-1.3/Quick_Magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick-Magic
-Version: 1.2
+Version: 1.3
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.2/README.md` & `Quick_Magic-1.3/README.md`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.2/setup.py` & `Quick_Magic-1.3/setup.py`

 * *Files identical despite different names*


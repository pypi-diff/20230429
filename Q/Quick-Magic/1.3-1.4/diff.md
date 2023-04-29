# Comparing `tmp/Quick_Magic-1.3.tar.gz` & `tmp/Quick_Magic-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quick_Magic-1.3.tar", last modified: Sat Apr 29 18:16:38 2023, max compression
+gzip compressed data, was "Quick_Magic-1.4.tar", last modified: Sat Apr 29 18:43:06 2023, max compression
```

## Comparing `Quick_Magic-1.3.tar` & `Quick_Magic-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:16:38.965930 Quick_Magic-1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 18:16:24.000000 Quick_Magic-1.3/Quick_Magic/update_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:16:38.965930 Quick_Magic-1.3/Quick_Magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:16:38.000000 Quick_Magic-1.3/Quick_Magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 18:16:24.000000 Quick_Magic-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:16:38.965930 Quick_Magic-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 18:16:24.000000 Quick_Magic-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:06.588420 Quick_Magic-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:43:06.588420 Quick_Magic-1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:06.588420 Quick_Magic-1.4/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 18:42:55.000000 Quick_Magic-1.4/Quick_Magic/update_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:43:06.588420 Quick_Magic-1.4/Quick_Magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 18:43:06.000000 Quick_Magic-1.4/Quick_Magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 18:43:06.000000 Quick_Magic-1.4/Quick_Magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:43:06.000000 Quick_Magic-1.4/Quick_Magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 18:43:06.000000 Quick_Magic-1.4/Quick_Magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:43:06.000000 Quick_Magic-1.4/Quick_Magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 18:42:55.000000 Quick_Magic-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:43:06.588420 Quick_Magic-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 18:42:55.000000 Quick_Magic-1.4/setup.py
```

### Comparing `Quick_Magic-1.3/PKG-INFO` & `Quick_Magic-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick_Magic
-Version: 1.3
+Version: 1.4
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.3/Quick_Magic/__init__.py` & `Quick_Magic-1.4/Quick_Magic/__init__.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.3/Quick_Magic/check.py` & `Quick_Magic-1.4/Quick_Magic/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     if check_data == False:
         os.mkdir(main_path)
         os.system(("attrib +h "+main_path))
     if print_text:
         print("LOADING APPS... (JUST ONCE)")
     cmd = 'powershell -ExecutionPolicy Bypass "Get-StartApps|convertto-json"'
     result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, encoding='utf-8')
+    # Exception if the result is Empty
+    if not result.stdout:
+        raise Exception("No output returned by the command")
     apps = json.loads(result.stdout)
     names = {}
     for each in apps:
         names.update({each['Name'].lower():each['AppID']})
     with open((os.path.join(main_path,"data.json")),"w") as outfile:
         json.dump(names,outfile,indent = 4)
     setup_files()
```

### Comparing `Quick_Magic-1.3/Quick_Magic/commands.py` & `Quick_Magic-1.4/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.3/Quick_Magic/features.py` & `Quick_Magic-1.4/Quick_Magic/features.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.3/Quick_Magic/update_list.py` & `Quick_Magic-1.4/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.3/Quick_Magic.egg-info/PKG-INFO` & `Quick_Magic-1.4/Quick_Magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quick-Magic
-Version: 1.3
+Version: 1.4
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
```

### Comparing `Quick_Magic-1.3/README.md` & `Quick_Magic-1.4/README.md`

 * *Files identical despite different names*

### Comparing `Quick_Magic-1.3/setup.py` & `Quick_Magic-1.4/setup.py`

 * *Files identical despite different names*


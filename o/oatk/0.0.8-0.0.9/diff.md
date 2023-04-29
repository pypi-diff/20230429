# Comparing `tmp/oatk-0.0.8.tar.gz` & `tmp/oatk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oatk-0.0.8.tar", last modified: Mon Apr 24 12:22:58 2023, max compression
+gzip compressed data, was "oatk-0.0.9.tar", last modified: Mon Apr 24 13:04:42 2023, max compression
```

## Comparing `oatk-0.0.8.tar` & `oatk-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.522445 oatk-0.0.8/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.515893 oatk-0.0.8/.github/
--rw-r--r--   0 xtof       (501) staff       (20)    21159 2023-04-24 10:48:41.000000 oatk-0.0.8/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.8/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      182 2023-04-24 12:21:52.000000 oatk-0.0.8/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 12:22:58.522286 oatk-0.0.8/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.516362 oatk-0.0.8/examples/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-24 11:18:52.000000 oatk-0.0.8/examples/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.8/examples/create-and-validate.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.516673 oatk-0.0.8/examples/google/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-03-25 10:56:05.000000 oatk-0.0.8/examples/google/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1538 2023-04-24 11:19:17.000000 oatk-0.0.8/examples/google/app.py
--rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.8/examples/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.516881 oatk-0.0.8/oatk/
--rw-r--r--   0 xtof       (501) staff       (20)     5538 2023-04-24 12:22:04.000000 oatk-0.0.8/oatk/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      751 2023-04-24 09:58:16.000000 oatk-0.0.8/oatk/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.518190 oatk-0.0.8/oatk/fake/
--rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.8/oatk/fake/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.8/oatk/fake/db.py
--rw-r--r--   0 xtof       (501) staff       (20)     7971 2022-10-16 09:03:05.000000 oatk-0.0.8/oatk/fake/routes.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.518858 oatk-0.0.8/oatk/fake/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.8/oatk/fake/static/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.8/oatk/fake/static/oatk.js
--rw-r--r--   0 xtof       (501) staff       (20)     1341 2022-10-16 14:49:57.000000 oatk-0.0.8/oatk/fake/static/style.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.521026 oatk-0.0.8/oatk/fake/templates/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.8/oatk/fake/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      459 2022-10-16 14:32:06.000000 oatk-0.0.8/oatk/fake/templates/authorize.html
--rw-r--r--   0 xtof       (501) staff       (20)      206 2022-10-16 14:31:57.000000 oatk-0.0.8/oatk/fake/templates/base.html
--rw-r--r--   0 xtof       (501) staff       (20)     1514 2022-10-16 14:51:49.000000 oatk-0.0.8/oatk/fake/templates/create_client.html
--rw-r--r--   0 xtof       (501) staff       (20)      249 2022-10-16 14:31:48.000000 oatk-0.0.8/oatk/fake/templates/dialog.html
--rw-r--r--   0 xtof       (501) staff       (20)      343 2022-10-16 14:49:16.000000 oatk-0.0.8/oatk/fake/templates/home.html
--rw-r--r--   0 xtof       (501) staff       (20)      254 2022-10-16 14:30:22.000000 oatk-0.0.8/oatk/fake/templates/login.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.521647 oatk-0.0.8/oatk/js/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2023-04-15 12:40:08.000000 oatk-0.0.8/oatk/js/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.521872 oatk-0.0.8/oatk/js/__pycache__/
--rw-r--r--   0 xtof       (501) staff       (20)      404 2023-04-15 12:40:48.000000 oatk-0.0.8/oatk/js/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 xtof       (501) staff       (20)    15655 2023-04-24 11:59:58.000000 oatk-0.0.8/oatk/js/oatk.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:22:58.517598 oatk-0.0.8/oatk.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      822 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       44 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       94 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       14 2023-04-24 12:22:58.000000 oatk-0.0.8/oatk.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-24 12:22:58.522485 oatk-0.0.8/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1582 2023-04-24 11:19:11.000000 oatk-0.0.8/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.654005 oatk-0.0.9/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.648053 oatk-0.0.9/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)    21159 2023-04-24 10:48:41.000000 oatk-0.0.9/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.9/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      182 2023-04-24 12:21:52.000000 oatk-0.0.9/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 13:04:42.653854 oatk-0.0.9/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.648489 oatk-0.0.9/examples/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-24 11:18:52.000000 oatk-0.0.9/examples/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.9/examples/create-and-validate.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.648804 oatk-0.0.9/examples/google/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-03-25 10:56:05.000000 oatk-0.0.9/examples/google/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1538 2023-04-24 11:19:17.000000 oatk-0.0.9/examples/google/app.py
+-rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.9/examples/web.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.648998 oatk-0.0.9/oatk/
+-rw-r--r--   0 xtof       (501) staff       (20)     5538 2023-04-24 13:03:49.000000 oatk-0.0.9/oatk/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      751 2023-04-24 09:58:16.000000 oatk-0.0.9/oatk/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.650231 oatk-0.0.9/oatk/fake/
+-rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.9/oatk/fake/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.9/oatk/fake/db.py
+-rw-r--r--   0 xtof       (501) staff       (20)     7971 2022-10-16 09:03:05.000000 oatk-0.0.9/oatk/fake/routes.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.650892 oatk-0.0.9/oatk/fake/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.9/oatk/fake/static/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.9/oatk/fake/static/oatk.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1341 2022-10-16 14:49:57.000000 oatk-0.0.9/oatk/fake/static/style.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.652664 oatk-0.0.9/oatk/fake/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.9/oatk/fake/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      459 2022-10-16 14:32:06.000000 oatk-0.0.9/oatk/fake/templates/authorize.html
+-rw-r--r--   0 xtof       (501) staff       (20)      206 2022-10-16 14:31:57.000000 oatk-0.0.9/oatk/fake/templates/base.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1514 2022-10-16 14:51:49.000000 oatk-0.0.9/oatk/fake/templates/create_client.html
+-rw-r--r--   0 xtof       (501) staff       (20)      249 2022-10-16 14:31:48.000000 oatk-0.0.9/oatk/fake/templates/dialog.html
+-rw-r--r--   0 xtof       (501) staff       (20)      343 2022-10-16 14:49:16.000000 oatk-0.0.9/oatk/fake/templates/home.html
+-rw-r--r--   0 xtof       (501) staff       (20)      254 2022-10-16 14:30:22.000000 oatk-0.0.9/oatk/fake/templates/login.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.653307 oatk-0.0.9/oatk/js/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2023-04-15 12:40:08.000000 oatk-0.0.9/oatk/js/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.653439 oatk-0.0.9/oatk/js/__pycache__/
+-rw-r--r--   0 xtof       (501) staff       (20)      404 2023-04-15 12:40:48.000000 oatk-0.0.9/oatk/js/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 xtof       (501) staff       (20)    15786 2023-04-24 13:02:56.000000 oatk-0.0.9/oatk/js/oatk.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 13:04:42.649696 oatk-0.0.9/oatk.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      822 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       44 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       94 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       14 2023-04-24 13:04:42.000000 oatk-0.0.9/oatk.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-24 13:04:42.654057 oatk-0.0.9/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1582 2023-04-24 11:19:11.000000 oatk-0.0.9/setup.py
```

### Comparing `oatk-0.0.8/.github/README.md` & `oatk-0.0.9/.github/README.md`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/LICENSE.txt` & `oatk-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/PKG-INFO` & `oatk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
```

### Comparing `oatk-0.0.8/examples/google/app.py` & `oatk-0.0.9/examples/google/app.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/examples/web.py` & `oatk-0.0.9/examples/web.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/__init__.py` & `oatk-0.0.9/oatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 import uuid
```

### Comparing `oatk-0.0.8/oatk/__main__.py` & `oatk-0.0.9/oatk/__main__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/__init__.py` & `oatk-0.0.9/oatk/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/db.py` & `oatk-0.0.9/oatk/fake/db.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/routes.py` & `oatk-0.0.9/oatk/fake/routes.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/static/oatk.js` & `oatk-0.0.9/oatk/fake/static/oatk.js`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/static/style.css` & `oatk-0.0.9/oatk/fake/static/style.css`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/fake/templates/create_client.html` & `oatk-0.0.9/oatk/fake/templates/create_client.html`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/oatk/js/oatk.js` & `oatk-0.0.9/oatk/js/oatk.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -258,15 +258,16 @@
             }
             if (after_logout) {
                 after_logout();
             }
         },
         callback = null;
 
-    // exposed function
+    // exposed functions
+
     var with_authenticated_user = function with_authenicated_user(on_success) {
         callback = on_success;
         flow(); // start flow
     }
 
     function have_authenticated_user() {
         return token != null;
@@ -313,28 +314,31 @@
                     return get_code();
                 }
                 console.log("✅ authorization code");
                 return get_token();
             }
         }
         console.log("✅ access token");
-        if (!callback) {
-            return alert("no callback?!");
-        }
 
         // we've got everyting...
-        callback(user_info_from_token(), http, logout);
+        if (callback) {
+            callback(user_info_from_token(), http, logout);
+        }
     }
 
     globals.oatk = {
         "using_provider": using_provider,
         "using_client_id": using_client_id,
         "apply_flow": apply_flow,
         "with_authenticated_user": with_authenticated_user,
-        "have_authenticated_user": have_authenticated_user
+        "have_authenticated_user": have_authenticated_user,
+        "get_user_info": user_info_from_token,
+        "http": http,
+        "login": flow,
+        "logout": logout
     };
 
 
     // helper
 
     /*
     Copyright 2022 Andrea Griffini
```

### Comparing `oatk-0.0.8/oatk.egg-info/PKG-INFO` & `oatk-0.0.9/oatk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
```

### Comparing `oatk-0.0.8/oatk.egg-info/SOURCES.txt` & `oatk-0.0.9/oatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oatk-0.0.8/setup.py` & `oatk-0.0.9/setup.py`

 * *Files identical despite different names*


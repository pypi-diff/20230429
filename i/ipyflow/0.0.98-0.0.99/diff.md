# Comparing `tmp/ipyflow-0.0.98.tar.gz` & `tmp/ipyflow-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyflow-0.0.98.tar", last modified: Mon Jun  6 01:56:13 2022, max compression
+gzip compressed data, was "ipyflow-0.0.99.tar", last modified: Mon Jun  6 21:52:20 2022, max compression
```

## Comparing `ipyflow-0.0.98.tar` & `ipyflow-0.0.99.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.880669 ipyflow-0.0.98/
--rw-r--r--   0 smacke     (501) staff       (20)    11136 2022-06-06 01:55:19.000000 ipyflow-0.0.98/HISTORY.rst
--rw-r--r--   0 smacke     (501) staff       (20)     1471 2022-03-26 16:21:58.000000 ipyflow-0.0.98/LICENSE.txt
--rw-r--r--   0 smacke     (501) staff       (20)      132 2022-03-27 18:08:14.000000 ipyflow-0.0.98/MANIFEST.in
--rw-r--r--   0 smacke     (501) staff       (20)     6985 2022-06-06 01:56:13.880766 ipyflow-0.0.98/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)     6207 2022-03-26 20:08:59.000000 ipyflow-0.0.98/README.md
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.871725 ipyflow-0.0.98/core/
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.871794 ipyflow-0.0.98/core/ipyflow/
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.872169 ipyflow-0.0.98/core/ipyflow/resources/
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.876147 ipyflow-0.0.98/core/ipyflow/resources/kernel/
--rw-r--r--   0 smacke     (501) staff       (20)      160 2022-03-27 04:57:08.000000 ipyflow-0.0.98/core/ipyflow/resources/kernel/kernel.json
--rw-r--r--   0 smacke     (501) staff       (20)     2329 2022-03-26 20:08:59.000000 ipyflow-0.0.98/core/ipyflow/resources/kernel/logo-32x32.png
--rw-r--r--   0 smacke     (501) staff       (20)     5018 2022-03-26 20:08:59.000000 ipyflow-0.0.98/core/ipyflow/resources/kernel/logo-64x64.png
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.876719 ipyflow-0.0.98/core/ipyflow/resources/labextension/
--rw-r--r--   0 smacke     (501) staff       (20)     2382 2022-06-06 01:55:45.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/package.json
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.877974 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/
--rw-r--r--   0 smacke     (501) staff       (20)     5072 2022-06-06 01:55:45.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/549.780992a9df8954c5e5b9.js
--rw-r--r--   0 smacke     (501) staff       (20)     5177 2022-06-06 01:55:45.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/568.5572cd4932d5900555fe.js
--rw-r--r--   0 smacke     (501) staff       (20)     6944 2022-06-06 01:55:45.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/remoteEntry.d15561f43418e6e10f48.js
--rw-r--r--   0 smacke     (501) staff       (20)      162 2022-06-06 01:55:44.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/style.js
--rw-r--r--   0 smacke     (501) staff       (20)     2452 2022-06-06 01:55:45.000000 ipyflow-0.0.98/core/ipyflow/resources/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.878748 ipyflow-0.0.98/core/ipyflow/resources/nbextension/
--rw-r--r--   0 smacke     (501) staff       (20)    14252 2022-06-06 01:55:57.000000 ipyflow-0.0.98/core/ipyflow/resources/nbextension/index.js
--rw-r--r--   0 smacke     (501) staff       (20)    42348 2022-06-06 01:55:57.000000 ipyflow-0.0.98/core/ipyflow/resources/nbextension/index.js.map
--rw-r--r--   0 smacke     (501) staff       (20)       57 2022-06-06 01:55:57.000000 ipyflow-0.0.98/core/ipyflow/resources/nbextension/ipyflow.json
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.881459 ipyflow-0.0.98/frontend/
--rw-r--r--   0 smacke     (501) staff       (20)      498 2022-06-06 01:56:13.881516 ipyflow-0.0.98/frontend/_version.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:13.880459 ipyflow-0.0.98/ipyflow.egg-info/
--rw-r--r--   0 smacke     (501) staff       (20)     6985 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)      963 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/SOURCES.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/dependency_links.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/not-zip-safe
--rw-r--r--   0 smacke     (501) staff       (20)      143 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/requires.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 01:56:13.000000 ipyflow-0.0.98/ipyflow.egg-info/top_level.txt
--rw-r--r--   0 smacke     (501) staff       (20)       54 2022-03-27 01:08:33.000000 ipyflow-0.0.98/requirements.txt
--rw-r--r--   0 smacke     (501) staff       (20)      272 2022-06-06 01:56:13.881184 ipyflow-0.0.98/setup.cfg
--rw-r--r--   0 smacke     (501) staff       (20)     2496 2022-04-17 02:14:02.000000 ipyflow-0.0.98/setup.py
--rw-r--r--   0 smacke     (501) staff       (20)    68611 2022-04-17 02:14:02.000000 ipyflow-0.0.98/versioneer.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.597656 ipyflow-0.0.99/
+-rw-r--r--   0 smacke     (501) staff       (20)    11258 2022-06-06 21:47:26.000000 ipyflow-0.0.99/HISTORY.rst
+-rw-r--r--   0 smacke     (501) staff       (20)     1471 2022-03-26 16:21:58.000000 ipyflow-0.0.99/LICENSE.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      132 2022-06-06 21:07:30.000000 ipyflow-0.0.99/MANIFEST.in
+-rw-r--r--   0 smacke     (501) staff       (20)     6985 2022-06-06 21:52:20.597825 ipyflow-0.0.99/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)     6207 2022-06-06 21:07:30.000000 ipyflow-0.0.99/README.md
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.588656 ipyflow-0.0.99/core/
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.588722 ipyflow-0.0.99/core/ipyflow/
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.589100 ipyflow-0.0.99/core/ipyflow/resources/
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.592367 ipyflow-0.0.99/core/ipyflow/resources/kernel/
+-rw-r--r--   0 smacke     (501) staff       (20)      160 2022-06-06 21:07:30.000000 ipyflow-0.0.99/core/ipyflow/resources/kernel/kernel.json
+-rw-r--r--   0 smacke     (501) staff       (20)     2329 2022-06-06 21:07:30.000000 ipyflow-0.0.99/core/ipyflow/resources/kernel/logo-32x32.png
+-rw-r--r--   0 smacke     (501) staff       (20)     5018 2022-06-06 21:07:30.000000 ipyflow-0.0.99/core/ipyflow/resources/kernel/logo-64x64.png
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.592745 ipyflow-0.0.99/core/ipyflow/resources/labextension/
+-rw-r--r--   0 smacke     (501) staff       (20)     2382 2022-06-06 21:51:53.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/package.json
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.594529 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/
+-rw-r--r--   0 smacke     (501) staff       (20)     5072 2022-06-06 21:51:53.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/549.780992a9df8954c5e5b9.js
+-rw-r--r--   0 smacke     (501) staff       (20)     5177 2022-06-06 21:51:53.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/568.5572cd4932d5900555fe.js
+-rw-r--r--   0 smacke     (501) staff       (20)     6944 2022-06-06 21:51:53.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/remoteEntry.152a06e5c2c89eacd270.js
+-rw-r--r--   0 smacke     (501) staff       (20)      162 2022-06-06 21:51:52.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/style.js
+-rw-r--r--   0 smacke     (501) staff       (20)     2452 2022-06-06 21:51:53.000000 ipyflow-0.0.99/core/ipyflow/resources/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.595440 ipyflow-0.0.99/core/ipyflow/resources/nbextension/
+-rw-r--r--   0 smacke     (501) staff       (20)    14252 2022-06-06 21:52:05.000000 ipyflow-0.0.99/core/ipyflow/resources/nbextension/index.js
+-rw-r--r--   0 smacke     (501) staff       (20)    42348 2022-06-06 21:52:05.000000 ipyflow-0.0.99/core/ipyflow/resources/nbextension/index.js.map
+-rw-r--r--   0 smacke     (501) staff       (20)       57 2022-06-06 21:52:05.000000 ipyflow-0.0.99/core/ipyflow/resources/nbextension/ipyflow.json
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.598948 ipyflow-0.0.99/frontend/
+-rw-r--r--   0 smacke     (501) staff       (20)      498 2022-06-06 21:52:20.599010 ipyflow-0.0.99/frontend/_version.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:52:20.597354 ipyflow-0.0.99/ipyflow.egg-info/
+-rw-r--r--   0 smacke     (501) staff       (20)     6985 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)      963 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/SOURCES.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/dependency_links.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/not-zip-safe
+-rw-r--r--   0 smacke     (501) staff       (20)      143 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/requires.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 21:52:20.000000 ipyflow-0.0.99/ipyflow.egg-info/top_level.txt
+-rw-r--r--   0 smacke     (501) staff       (20)       54 2022-06-06 21:07:30.000000 ipyflow-0.0.99/requirements.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      272 2022-06-06 21:52:20.598532 ipyflow-0.0.99/setup.cfg
+-rw-r--r--   0 smacke     (501) staff       (20)     2496 2022-06-06 21:07:30.000000 ipyflow-0.0.99/setup.py
+-rw-r--r--   0 smacke     (501) staff       (20)    68611 2022-04-17 02:14:02.000000 ipyflow-0.0.99/versioneer.py
```

### Comparing `ipyflow-0.0.98/HISTORY.rst` & `ipyflow-0.0.99/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 History
 =======
 
+0.0.99 (2022-06-06)
+-------------------
+* Fix serialization bug that prevented in-order semantics from working properly;
+
 0.0.98 (2022-06-05)
 -------------------
 * Add ability to register custom comm handlers;
 * Fix lazy import ImportError issue (possibly manifesting on cinder);
 
 0.0.97 (2022-05-30)
 -------------------
```

### Comparing `ipyflow-0.0.98/LICENSE.txt` & `ipyflow-0.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/PKG-INFO` & `ipyflow-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyflow
-Version: 0.0.98
+Version: 0.0.99
 Summary: Fearless interactivity for Jupyter notebooks.
 Home-page: https://github.com/nbsafety-project/nbsafety
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipyflow-0.0.98/README.md` & `ipyflow-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/kernel/logo-32x32.png` & `ipyflow-0.0.99/core/ipyflow/resources/kernel/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/kernel/logo-64x64.png` & `ipyflow-0.0.99/core/ipyflow/resources/kernel/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/labextension/package.json` & `ipyflow-0.0.99/core/ipyflow/resources/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714506172839505%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.152a06e5c2c89eacd270.js'}}",*

 * * "'version'": "'0.0.99'"}*

```diff
@@ -27,15 +27,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbsafety-project/nbsafety",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d15561f43418e6e10f48.js",
+            "load": "static/remoteEntry.152a06e5c2c89eacd270.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../core/ipyflow/resources/labextension/"
     },
     "keywords": [
         "jupyter",
@@ -66,9 +66,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.0.98"
+    "version": "0.0.99"
 }
```

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/labextension/static/549.780992a9df8954c5e5b9.js` & `ipyflow-0.0.99/core/ipyflow/resources/labextension/static/549.780992a9df8954c5e5b9.js`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/labextension/static/568.5572cd4932d5900555fe.js` & `ipyflow-0.0.99/core/ipyflow/resources/labextension/static/568.5572cd4932d5900555fe.js`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/labextension/static/remoteEntry.d15561f43418e6e10f48.js` & `ipyflow-0.0.99/core/ipyflow/resources/labextension/static/remoteEntry.152a06e5c2c89eacd270.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(568).then((() => () => k(568))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-ipyflow", "0.0.98"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-ipyflow", "0.0.99"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/labextension/static/third-party-licenses.json` & `ipyflow-0.0.99/core/ipyflow/resources/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/nbextension/index.js` & `ipyflow-0.0.99/core/ipyflow/resources/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/core/ipyflow/resources/nbextension/index.js.map` & `ipyflow-0.0.99/core/ipyflow/resources/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/ipyflow.egg-info/PKG-INFO` & `ipyflow-0.0.99/ipyflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyflow
-Version: 0.0.98
+Version: 0.0.99
 Summary: Fearless interactivity for Jupyter notebooks.
 Home-page: https://github.com/nbsafety-project/nbsafety
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipyflow-0.0.98/setup.py` & `ipyflow-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `ipyflow-0.0.98/versioneer.py` & `ipyflow-0.0.99/versioneer.py`

 * *Files identical despite different names*


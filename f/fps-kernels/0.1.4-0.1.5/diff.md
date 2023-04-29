# Comparing `tmp/fps_kernels-0.1.4.tar.gz` & `tmp/fps_kernels-0.1.5.tar.gz`

## Comparing `fps_kernels-0.1.4.tar` & `fps_kernels-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/main.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/COPYING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/main.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/COPYING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.5/PKG-INFO
```

### Comparing `fps_kernels-0.1.4/fps_kernels/main.py` & `fps_kernels-0.1.5/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/routes.py` & `fps_kernels-0.1.5/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_driver/connect.py` & `fps_kernels-0.1.5/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_driver/driver.py` & `fps_kernels-0.1.5/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_driver/kernelspec.py` & `fps_kernels-0.1.5/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_driver/message.py` & `fps_kernels-0.1.5/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_driver/paths.py` & `fps_kernels-0.1.5/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_server/message.py` & `fps_kernels-0.1.5/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/fps_kernels/kernel_server/server.py` & `fps_kernels-0.1.5/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/.gitignore` & `fps_kernels-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/COPYING.md` & `fps_kernels-0.1.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/pyproject.toml` & `fps_kernels-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.4/PKG-INFO` & `fps_kernels-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_kernels
-Version: 0.1.4
+Version: 0.1.5
 Summary: An FPS plugin for the kernels API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```


# Comparing `tmp/envoy.gpg.identity-0.1.0.tar.gz` & `tmp/envoy.gpg.identity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.gpg.identity-0.1.0.tar", last modified: Tue Mar  1 08:46:47 2022, max compression
+gzip compressed data, was "envoy.gpg.identity-0.1.1.tar", last modified: Sat Apr 29 18:12:01 2023, max compression
```

## Comparing `envoy.gpg.identity-0.1.0.tar` & `envoy.gpg.identity-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/envoy/gpg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/envoy/gpg/identity/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy/gpg/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy/gpg/identity/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy/gpg/identity/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/envoy.gpg.identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-01 08:46:47.650234 envoy.gpg.identity-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-03-01 08:46:47.000000 envoy.gpg.identity-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.925363 envoy.gpg.identity-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-29 18:12:01.925363 envoy.gpg.identity-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.921363 envoy.gpg.identity-0.1.1/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.921363 envoy.gpg.identity-0.1.1/envoy/gpg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.925363 envoy.gpg.identity-0.1.1/envoy/gpg/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy/gpg/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy/gpg/identity/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy/gpg/identity/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:12:01.921363 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/envoy.gpg.identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:12:01.925363 envoy.gpg.identity-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-29 18:12:01.000000 envoy.gpg.identity-0.1.1/setup.py
```

### Comparing `envoy.gpg.identity-0.1.0/backend_shim.py` & `envoy.gpg.identity-0.1.1/backend_shim.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
+os.makedirs(dist_dir, exist_ok=True)
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `envoy.gpg.identity-0.1.0/envoy/gpg/identity/identity.py` & `envoy.gpg.identity-0.1.1/envoy/gpg/identity/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,17 @@
 
     @cached_property
     def provided_id(self) -> Optional[str]:
         """Provided name and/or email for the identity."""
         if not (self.provided_name or self.provided_email):
             return None
         return (
-            formataddr((self.provided_name, self.provided_email))
+            formataddr(
+                (self.provided_name,
+                 self.provided_email)).replace('"', "")
             if (self.provided_name and self.provided_email)
             else (self.provided_name or self.provided_email))
 
     @property
     def provided_name(self) -> Optional[str]:
         """Provided name for the identity."""
         return self._provided_name
```

### Comparing `envoy.gpg.identity-0.1.0/setup.py` & `envoy.gpg.identity-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 setup(**{
     'author': 'Ryan Northey',
     'author_email': 'ryan@synca.io',
     'description': '"GPG identity util used in Envoy proxy\'s CI"',
     'install_requires': (
-        'aio.core>=0.8.0',
+        'aio.core>=0.10.0',
         'python-gnupg',
     ),
     'license': 'Apache Software License 2.0',
     'long_description': """
 envoy.gpg.identity
 ==================
 
@@ -28,10 +28,11 @@
         'envoy.gpg.identity': (
             'py.typed',
         ),
     },
     'packages': (
         'envoy.gpg.identity',
     ),
+    'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.gpg.identity',
-    'version': '0.1.0',
+    'version': '0.1.1',
 })
```


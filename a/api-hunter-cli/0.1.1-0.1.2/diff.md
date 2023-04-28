# Comparing `tmp/api-hunter-cli-0.1.1.tar.gz` & `tmp/api_hunter_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-hunter-cli-0.1.1.tar", last modified: Fri Apr 28 22:09:36 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.2.tar", last modified: Fri Apr 28 22:43:00 2023, max compression
```

## Comparing `api-hunter-cli-0.1.1.tar` & `api_hunter_cli-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api-hunter-cli-0.1.1/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/api_hunter/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api-hunter-cli-0.1.1/api_hunter/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api-hunter-cli-0.1.1/api_hunter/main.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      290 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       49 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       11 2023-04-28 22:09:36.000000 api-hunter-cli-0.1.1/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:09:36.934436 api-hunter-cli-0.1.1/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1323 2023-04-28 22:09:28.000000 api-hunter-cli-0.1.1/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:43:00.413982 api_hunter_cli-0.1.2/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:43:00.413982 api_hunter_cli-0.1.2/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.2/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:43:00.413982 api_hunter_cli-0.1.2/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.2/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api_hunter_cli-0.1.2/api_hunter_cli/main.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:43:00.413982 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      298 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       54 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 22:43:00.000000 api_hunter_cli-0.1.2/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:43:00.413982 api_hunter_cli-0.1.2/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1333 2023-04-28 22:42:05.000000 api_hunter_cli-0.1.2/setup.py
```

### Comparing `api-hunter-cli-0.1.1/PKG-INFO` & `api_hunter_cli-0.1.2/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api-hunter-cli-0.1.1/api_hunter/main.py` & `api_hunter_cli-0.1.2/api_hunter_cli/main.py`

 * *Files identical despite different names*

### Comparing `api-hunter-cli-0.1.1/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: api-hunter-cli
-Version: 0.1.1
+Name: api_hunter_cli
+Version: 0.1.2
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api-hunter-cli-0.1.1/setup.py` & `api_hunter_cli-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
-    name="api-hunter-cli",
-    version="0.1.1",
+    name="api_hunter_cli",
+    version="0.1.2",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
         "typer[all]",
         "yaspin",
         "inquirer",
     ],
     entry_points={
         "console_scripts": [
-            "apihunt=api_hunter.main:main",
+            "apihunter=apihunter.__main__:main",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -38,9 +38,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.7",
-    cmdclass={"install": PostInstallCommand},
+    cmdclass={"post_install": PostInstallCommand},
 )
```


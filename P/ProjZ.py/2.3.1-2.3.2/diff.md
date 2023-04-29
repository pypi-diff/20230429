# Comparing `tmp/ProjZ.py-2.3.1.tar.gz` & `tmp/ProjZ.py-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.3.1.tar", last modified: Sat Apr 29 12:18:35 2023, max compression
+gzip compressed data, was "ProjZ.py-2.3.2.tar", last modified: Sat Apr 29 12:23:47 2023, max compression
```

## Comparing `ProjZ.py-2.3.1.tar` & `ProjZ.py-2.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:18:35.312546 ProjZ.py-2.3.1/
--rw-rw-rw-   0        0        0     3981 2023-04-29 12:18:35.313509 ProjZ.py-2.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:18:35.311530 ProjZ.py-2.3.1/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     3981 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 12:18:35.315160 ProjZ.py-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2021 2023-04-29 12:18:31.000000 ProjZ.py-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:23:47.666493 ProjZ.py-2.3.2/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 12:23:47.667463 ProjZ.py-2.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 12:23:47.664470 ProjZ.py-2.3.2/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 12:23:47.000000 ProjZ.py-2.3.2/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-29 12:23:47.000000 ProjZ.py-2.3.2/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:23:47.000000 ProjZ.py-2.3.2/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-29 12:23:47.000000 ProjZ.py-2.3.2/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:23:47.000000 ProjZ.py-2.3.2/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:23:47.669059 ProjZ.py-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2024 2023-04-29 12:23:44.000000 ProjZ.py-2.3.2/setup.py
```

### Comparing `ProjZ.py-2.3.1/PKG-INFO` & `ProjZ.py-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.1
+Version: 2.3.2
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
-Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-botprojz-botsprojz-api
+Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ProjZ
 A simple asynchronous library for interaction with Project Z
```

### Comparing `ProjZ.py-2.3.1/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.3.2/ProjZ.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.1
+Version: 2.3.2
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
-Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-botprojz-botsprojz-api
+Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ProjZ
 A simple asynchronous library for interaction with Project Z
```

### Comparing `ProjZ.py-2.3.1/README.md` & `ProjZ.py-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.1/setup.py` & `ProjZ.py-2.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,26 @@
                     print("Installation canceled.")
                     return
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.3.1",
+        version="2.3.2",
         author="D4krwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
         python_requires=">=3.7",
         keywords=[
             "project-z", "projectz", "projz",
             "bots", "api", "supersymlab",
-            "projz-bot" "projz-bots" "projz-api"
+            "projz-bot", "projz-bots", "projz-api",
         ]
     )
 
 
 if __name__ == "__main__":
     main()
```


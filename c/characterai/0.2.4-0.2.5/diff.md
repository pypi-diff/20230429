# Comparing `tmp/characterai-0.2.4.tar.gz` & `tmp/characterai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.2.4.tar", last modified: Sat Apr 29 10:49:05 2023, max compression
+gzip compressed data, was "dist\characterai-0.2.5.tar", last modified: Sat Apr 29 11:51:41 2023, max compression
```

## Comparing `characterai-0.2.4.tar` & `characterai-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:49:05.455299 characterai-0.2.4/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      455 2023-04-29 10:49:05.454297 characterai-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 characterai-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:49:05.387158 characterai-0.2.4/characterai/
--rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.2.4/characterai/__init__.py
--rw-rw-rw-   0        0        0     9360 2023-04-29 10:38:10.000000 characterai-0.2.4/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.2.4/characterai/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:49:05.450296 characterai-0.2.4/characterai.egg-info/
--rw-rw-rw-   0        0        0      455 2023-04-29 10:49:05.000000 characterai-0.2.4/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-29 10:49:05.000000 characterai-0.2.4/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:49:05.000000 characterai-0.2.4/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-29 10:49:05.000000 characterai-0.2.4/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 10:49:05.000000 characterai-0.2.4/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:49:05.456299 characterai-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-04-29 10:47:57.000000 characterai-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.548015 characterai-0.2.5/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      455 2023-04-29 11:51:41.546014 characterai-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 characterai-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.495013 characterai-0.2.5/characterai/
+-rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.2.5/characterai/__init__.py
+-rw-rw-rw-   0        0        0     9358 2023-04-29 11:50:04.000000 characterai-0.2.5/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.2.5/characterai/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.543018 characterai-0.2.5/characterai.egg-info/
+-rw-rw-rw-   0        0        0      455 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:51:41.548015 characterai-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-04-29 11:51:38.000000 characterai-0.2.5/setup.py
```

### Comparing `characterai-0.2.4/LICENSE` & `characterai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.2.4/characterai/characterai.py` & `characterai-0.2.5/characterai/characterai.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.user = self.user()
         self.character = self.character()
         self.chat = self.chat()
 
     async def init(self):
         global page
 
-        self.browser = await (await async_playwright().start()).firefox.launch(headless=False)
+        self.browser = await (await async_playwright().start()).firefox.launch(headless=True)
         self.context = await self.browser.new_context(extra_http_headers={"Authorization": f"Token {self.token}"})
         page = await self.context.new_page()
 
     # [FOR LIBRARY] Convert site to json
     async def GetResponse(link: str) -> Dict[str, str]:
         await pyAsyncCAI.goto(f'https://beta.character.ai/{link}/')
         data = json.loads(await (page.locator('pre').inner_text()))
@@ -134,15 +134,15 @@
 
 
 class pyCAI:
     def __init__(self, token: str):
         global page
 
         self.token = token
-        self.browser = sync_playwright().start().firefox.launch(headless=False)
+        self.browser = sync_playwright().start().firefox.launch(headless=True)
         self.context = self.browser.new_context(
             extra_http_headers={"Authorization": f"Token {self.token}"})
         page = self.context.new_page()
 
         self.user = self.user()
         self.character = self.character()
         self.chat = self.chat()
```

### Comparing `characterai-0.2.4/setup.py` & `characterai-0.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='characterai',
-    version='0.2.4',
+    version='0.2.5',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/characterai',
     packages=find_packages(),
     install_requires=["playwright==1.32.1"],
```


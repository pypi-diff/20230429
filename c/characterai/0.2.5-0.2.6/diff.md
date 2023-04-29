# Comparing `tmp/characterai-0.2.5.tar.gz` & `tmp/characterai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.2.5.tar", last modified: Sat Apr 29 11:51:41 2023, max compression
+gzip compressed data, was "characterai-0.2.6.tar", last modified: Sat Apr 29 18:36:41 2023, max compression
```

## Comparing `characterai-0.2.5.tar` & `characterai-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.548015 characterai-0.2.5/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      455 2023-04-29 11:51:41.546014 characterai-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 characterai-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.495013 characterai-0.2.5/characterai/
--rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.2.5/characterai/__init__.py
--rw-rw-rw-   0        0        0     9358 2023-04-29 11:50:04.000000 characterai-0.2.5/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.2.5/characterai/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:51:41.543018 characterai-0.2.5/characterai.egg-info/
--rw-rw-rw-   0        0        0      455 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 11:51:41.000000 characterai-0.2.5/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 11:51:41.548015 characterai-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-04-29 11:51:38.000000 characterai-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-29 18:28:44.000000 characterai-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 18:36:41.687003 characterai-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-04-29 18:28:44.000000 characterai-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/characterai/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-29 18:28:44.000000 characterai-0.2.6/characterai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-04-29 18:32:10.000000 characterai-0.2.6/characterai/characterai.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-29 18:28:44.000000 characterai-0.2.6/characterai/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/characterai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:36:41.687003 characterai-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      631 2023-04-29 18:36:32.000000 characterai-0.2.6/setup.py
```

### Comparing `characterai-0.2.5/LICENSE` & `characterai-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.2.5/characterai/characterai.py` & `characterai-0.2.6/characterai/characterai.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,22 +144,22 @@
         page = self.context.new_page()
 
         self.user = self.user()
         self.character = self.character()
         self.chat = self.chat()
 
     # [FOR LIBRARY] Convert site to json
-    def _GetResponse(link: str) -> Dict[str, str]:
+    def GetResponse(link: str) -> Dict[str, str]:
         pyCAI.goto(f'https://beta.character.ai/{link}/')
         data = json.loads(page.locator('pre').inner_text())
 
         return data
 
     # [FOR LIBRARY] Checking the page if it runs for the first time
-    def _goto(link: str):
+    def goto(link: str):
         page.goto(link)
 
         if page.title() != 'Waiting Room powered by Cloudflare':
             if page.get_by_role("button", name="Accept").is_visible():
                 page.get_by_role("button", name="Accept").click()
 
                 return page
```


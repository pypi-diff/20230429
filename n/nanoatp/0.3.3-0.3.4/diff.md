# Comparing `tmp/nanoatp-0.3.3.tar.gz` & `tmp/nanoatp-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.3.3.tar", max compression
+gzip compressed data, was "nanoatp-0.3.4.tar", max compression
```

## Comparing `nanoatp-0.3.3.tar` & `nanoatp-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.3/LICENSE
--rw-r--r--   0        0        0     4416 2023-04-29 17:13:39.380619 nanoatp-0.3.3/README.md
--rw-r--r--   0        0        0      283 2023-04-29 17:13:39.382268 nanoatp-0.3.3/nanoatp/__init__.py
--rw-r--r--   0        0        0     8669 2023-04-29 17:13:39.383183 nanoatp-0.3.3/nanoatp/bskyagent.py
--rw-r--r--   0        0        0     3034 2023-04-26 09:39:42.752327 nanoatp-0.3.3/nanoatp/richtext.py
--rw-r--r--   0        0        0      888 2023-04-29 17:13:39.384236 nanoatp-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 nanoatp-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4631 2023-04-29 17:30:20.383087 nanoatp-0.3.4/README.md
+-rw-r--r--   0        0        0      283 2023-04-29 17:30:20.383570 nanoatp-0.3.4/nanoatp/__init__.py
+-rw-r--r--   0        0        0     8669 2023-04-29 17:13:39.383183 nanoatp-0.3.4/nanoatp/bskyagent.py
+-rw-r--r--   0        0        0     3034 2023-04-26 09:39:42.752327 nanoatp-0.3.4/nanoatp/richtext.py
+-rw-r--r--   0        0        0      888 2023-04-29 17:30:20.384482 nanoatp-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 nanoatp-0.3.4/PKG-INFO
```

### Comparing `nanoatp-0.3.3/LICENSE` & `nanoatp-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.3/README.md` & `nanoatp-0.3.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 A nano implementation of the AT Protocol for Python.
 
 ## Demo
 
 - A bot built with nanoatp that summarizes the top 30 most popular arXiv papers on Reddit and Hacker News in the last 30 days and posts them to Bluesky.
   - [@paper.bsky.social](https://staging.bsky.app/profile/paper.bsky.social)
+    - It needs to have an account on Bluesky to see the posts. But there is a similar bot on Twitter [@susumuota](https://twitter.com/susumuota).
+  - [Source code](https://github.com/susumuota/arxiv-reddit-summary)
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
 pip install nanoatp
```

### Comparing `nanoatp-0.3.3/nanoatp/bskyagent.py` & `nanoatp-0.3.4/nanoatp/bskyagent.py`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.3/nanoatp/richtext.py` & `nanoatp-0.3.4/nanoatp/richtext.py`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.3/pyproject.toml` & `nanoatp-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.3.3"
+version = "0.3.4"
 description = "A nano implementation of the AT Protocol for Python."
 license = "MIT"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/susumuota/nanoatp"
 repository = "https://github.com/susumuota/nanoatp"
 documentation = "https://github.com/susumuota/nanoatp#readme"
```

### Comparing `nanoatp-0.3.3/PKG-INFO` & `nanoatp-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.3.3
+Version: 0.3.4
 Summary: A nano implementation of the AT Protocol for Python.
 Home-page: https://github.com/susumuota/nanoatp
 License: MIT
 Keywords: atprotocol,atproto,bluesky
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
 Requires-Python: >=3.9.16,<4.0.0
@@ -32,14 +32,16 @@
 
 A nano implementation of the AT Protocol for Python.
 
 ## Demo
 
 - A bot built with nanoatp that summarizes the top 30 most popular arXiv papers on Reddit and Hacker News in the last 30 days and posts them to Bluesky.
   - [@paper.bsky.social](https://staging.bsky.app/profile/paper.bsky.social)
+    - It needs to have an account on Bluesky to see the posts. But there is a similar bot on Twitter [@susumuota](https://twitter.com/susumuota).
+  - [Source code](https://github.com/susumuota/arxiv-reddit-summary)
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
 pip install nanoatp
```


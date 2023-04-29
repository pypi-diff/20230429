# Comparing `tmp/nanoatp-0.3.2.tar.gz` & `tmp/nanoatp-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.3.2.tar", max compression
+gzip compressed data, was "nanoatp-0.3.3.tar", max compression
```

## Comparing `nanoatp-0.3.2.tar` & `nanoatp-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.2/LICENSE
--rw-r--r--   0        0        0     4182 2023-04-23 09:33:59.603773 nanoatp-0.3.2/README.md
--rw-r--r--   0        0        0      283 2023-04-23 09:33:59.605564 nanoatp-0.3.2/nanoatp/__init__.py
--rw-r--r--   0        0        0     8539 2023-04-23 09:33:59.606360 nanoatp-0.3.2/nanoatp/bskyagent.py
--rw-r--r--   0        0        0     3034 2023-04-23 09:09:57.876090 nanoatp-0.3.2/nanoatp/richtext.py
--rw-r--r--   0        0        0      922 2023-04-23 09:33:59.607197 nanoatp-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 nanoatp-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4416 2023-04-29 17:13:39.380619 nanoatp-0.3.3/README.md
+-rw-r--r--   0        0        0      283 2023-04-29 17:13:39.382268 nanoatp-0.3.3/nanoatp/__init__.py
+-rw-r--r--   0        0        0     8669 2023-04-29 17:13:39.383183 nanoatp-0.3.3/nanoatp/bskyagent.py
+-rw-r--r--   0        0        0     3034 2023-04-26 09:39:42.752327 nanoatp-0.3.3/nanoatp/richtext.py
+-rw-r--r--   0        0        0      888 2023-04-29 17:13:39.384236 nanoatp-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 nanoatp-0.3.3/PKG-INFO
```

### Comparing `nanoatp-0.3.2/LICENSE` & `nanoatp-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.2/README.md` & `nanoatp-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 [![GitHub last commit](https://img.shields.io/github/last-commit/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/commits)
 &emsp;
 EN |
 [JA](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp) |
 [ES](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp) |
 [ZH](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=zh-CN&_x_tr_hl=zh-CN&_x_tr_pto=wapp)
 
-A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
+A nano implementation of the AT Protocol for Python.
+
+## Demo
+
+- A bot built with nanoatp that summarizes the top 30 most popular arXiv papers on Reddit and Hacker News in the last 30 days and posts them to Bluesky.
+  - [@paper.bsky.social](https://staging.bsky.app/profile/paper.bsky.social)
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
 pip install nanoatp
@@ -43,15 +48,15 @@
 rt = RichText("Hello @ota.bsky.social, check out this link: https://example.com")
 rt.detectFacets(agent)
 print(rt.facets)
 
 # upload an image
 image = agent.uploadImage("example.png")
 
-# post it
+# post a RichText with an image
 embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
 record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 response = agent.post(record)
 print(response)
 ```
 
 See [examples](https://github.com/susumuota/nanoatp/tree/main/examples) for more.
@@ -114,15 +119,15 @@
 ### Advanced API calls
 
 The methods above are convenience wrappers. It covers most but not all available methods.
 
 The AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:
 
 ```python
-res1 = agent.createRecord(
+res1 = agent._repo_createRecord(
     agent.session["did"],  # repo
     "app.bsky.feed.post",  # collection
     {
         "$type": "app.bsky.feed.post",
         "text": "Hello, world!",
         "createdAt": datetime.datetime.now(datetime.timezone.utc).isoformat().replace("+00:00", "Z")
     }
```

### Comparing `nanoatp-0.3.2/nanoatp/bskyagent.py` & `nanoatp-0.3.3/nanoatp/bskyagent.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,18 @@
             self.headers = {}
             raise Exception(str(session))
         self.session = session
         accessJwt = self.session.get("accessJwt")
         self.headers = {"Authorization": f"Bearer {accessJwt}"}
         return self.session
 
-    def getPost(self, repo: str, rkey: str, cid: str = "") -> dict[str, Any]:
+    def getPost(self, repo: str, rkey: str, cid: str = ""):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/bsky-agent.ts"""
+        if not self.session:
+            raise Exception("Not logged in")
         return self._repo_getRecord(repo, "app.bsky.feed.post", rkey, cid)
 
     def post(self, record: dict[str, Any]):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/bsky-agent.ts"""
         if not self.session:
             raise Exception("Not logged in")
         if not record.get("createdAt"):
@@ -55,22 +57,24 @@
         if not self.session:
             raise Exception("Not logged in")
         repo, collection, rkey = parseAtUri(postUri)
         if not (repo and collection and rkey):
             raise Exception(f"Invalid postUrl format: {postUri}")
         return self._repo_deleteRecord(repo, collection, rkey)
 
-    def uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
+    def uploadBlob(self, data: bytes, encoding: str):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/agent.ts"""
         if not self.session:
             raise Exception("Not logged in")
         return self._repo_uploadBlob(data, encoding)
 
     def resolveHandle(self, handle: str):
         """https://github.com/bluesky-social/atproto/blob/main/packages/api/src/agent.ts"""
+        if not self.session:
+            raise Exception("Not logged in")
         return self._identity_resolveHandle(handle)
 
     def uploadImage(self, path: str, alt: str = "", encoding: str = ""):
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/app/bsky/embed/images.json"""
         if not self.session:
             raise Exception("Not logged in")
         encoding = encoding or guess_type(path)[0] or "application/octet-stream"
@@ -164,15 +168,15 @@
     def _repo_uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/repo/uploadBlob.json"""
         headers = {"Content-Type": encoding, "Content-Length": str(len(data))}
         headers.update(self.headers)
         response = self.requests.post(f"{self.service}/xrpc/com.atproto.repo.uploadBlob", headers=headers, data=data)
         return response.json()
 
-    def _identity_resolveHandle(self, handle: str):
+    def _identity_resolveHandle(self, handle: str) -> dict[str, str]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/identity/resolveHandle.json"""
         params = {"handle": handle}
         response = self.requests.get(
             f"{self.service}/xrpc/com.atproto.identity.resolveHandle", headers=self.headers, params=params
         )
         return response.json()
```

### Comparing `nanoatp-0.3.2/nanoatp/richtext.py` & `nanoatp-0.3.3/nanoatp/richtext.py`

 * *Files identical despite different names*

### Comparing `nanoatp-0.3.2/pyproject.toml` & `nanoatp-0.3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.3.2"
-description = "A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python."
+version = "0.3.3"
+description = "A nano implementation of the AT Protocol for Python."
 license = "MIT"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/susumuota/nanoatp"
 repository = "https://github.com/susumuota/nanoatp"
 documentation = "https://github.com/susumuota/nanoatp#readme"
 keywords = ["atprotocol", "atproto", "bluesky"]
```

### Comparing `nanoatp-0.3.2/PKG-INFO` & `nanoatp-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.3.2
-Summary: A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
+Version: 0.3.3
+Summary: A nano implementation of the AT Protocol for Python.
 Home-page: https://github.com/susumuota/nanoatp
 License: MIT
 Keywords: atprotocol,atproto,bluesky
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
 Requires-Python: >=3.9.16,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,20 @@
 [![GitHub last commit](https://img.shields.io/github/last-commit/susumuota/nanoatp)](https://github.com/susumuota/nanoatp/commits)
 &emsp;
 EN |
 [JA](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=ja&_x_tr_hl=ja&_x_tr_pto=wapp) |
 [ES](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp) |
 [ZH](https://github-com.translate.goog/susumuota/nanoatp/blob/main/README.md?_x_tr_sl=en&_x_tr_tl=zh-CN&_x_tr_hl=zh-CN&_x_tr_pto=wapp)
 
-A nano implementation of the AT Protocol (Authenticated Transfer Protocol) for Python.
+A nano implementation of the AT Protocol for Python.
+
+## Demo
+
+- A bot built with nanoatp that summarizes the top 30 most popular arXiv papers on Reddit and Hacker News in the last 30 days and posts them to Bluesky.
+  - [@paper.bsky.social](https://staging.bsky.app/profile/paper.bsky.social)
 
 ## Getting started
 
 - First, install the package.
 
 ```bash
 pip install nanoatp
@@ -64,15 +69,15 @@
 rt = RichText("Hello @ota.bsky.social, check out this link: https://example.com")
 rt.detectFacets(agent)
 print(rt.facets)
 
 # upload an image
 image = agent.uploadImage("example.png")
 
-# post it
+# post a RichText with an image
 embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
 record = {"text": rt.text, "facets": rt.facets, "embed": embed}
 response = agent.post(record)
 print(response)
 ```
 
 See [examples](https://github.com/susumuota/nanoatp/tree/main/examples) for more.
@@ -135,15 +140,15 @@
 ### Advanced API calls
 
 The methods above are convenience wrappers. It covers most but not all available methods.
 
 The AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:
 
 ```python
-res1 = agent.createRecord(
+res1 = agent._repo_createRecord(
     agent.session["did"],  # repo
     "app.bsky.feed.post",  # collection
     {
         "$type": "app.bsky.feed.post",
         "text": "Hello, world!",
         "createdAt": datetime.datetime.now(datetime.timezone.utc).isoformat().replace("+00:00", "Z")
     }
```


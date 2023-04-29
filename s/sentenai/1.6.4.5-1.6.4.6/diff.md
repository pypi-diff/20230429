# Comparing `tmp/sentenai-1.6.4.5.tar.gz` & `tmp/sentenai-1.6.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentenai-1.6.4.5.tar", last modified: Fri Apr 28 20:33:56 2023, max compression
+gzip compressed data, was "sentenai-1.6.4.6.tar", last modified: Sat Apr 29 11:29:13 2023, max compression
```

## Comparing `sentenai-1.6.4.5.tar` & `sentenai-1.6.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.869784 sentenai-1.6.4.5/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.5/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-28 20:33:56.869864 sentenai-1.6.4.5/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.5/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.868024 sentenai-1.6.4.5/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9160 2023-04-27 15:19:47.000000 sentenai-1.6.4.5/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9729 2023-03-30 18:29:31.000000 sentenai-1.6.4.5/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.869585 sentenai-1.6.4.5/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.5/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.5/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.5/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24241 2023-04-28 20:33:48.000000 sentenai-1.6.4.5/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-28 20:33:56.868715 sentenai-1.6.4.5/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-28 20:33:56.000000 sentenai-1.6.4.5/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-28 20:33:56.870080 sentenai-1.6.4.5/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-28 20:33:48.000000 sentenai-1.6.4.5/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.593172 sentenai-1.6.4.6/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.6/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-29 11:29:13.593247 sentenai-1.6.4.6/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.6/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.591657 sentenai-1.6.4.6/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9068 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.593016 sentenai-1.6.4.6/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.6/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.6/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.6/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24627 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.592201 sentenai-1.6.4.6/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-29 11:29:13.593482 sentenai-1.6.4.6/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/setup.py
```

### Comparing `sentenai-1.6.4.5/LICENSE` & `sentenai-1.6.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.5/PKG-INFO` & `sentenai-1.6.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.5
+Version: 1.6.4.6
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.5/README.md` & `sentenai-1.6.4.6/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.5/sentenai/__init__.py` & `sentenai-1.6.4.6/sentenai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,26 @@
 __all__ = ['Sentenai']
 
 if PANDAS:
     def df(events):
         return pd.DataFrame([x.as_record() for x in events])
 
 class Sentenai(API):
-    def __init__(self, host=None, port=None, check=True, auth=None):
+    def __init__(self, host=None, port=None, check=True, interactive=True):
         ## We do this so we can programmatically pass in host/port
         if host is None:
             host = 'localhost'
         if port is None:
-            if auth:
-                port = 443
-            else:
-                port = 7280
-        if auth:
-            protocol = 'https://'
-        else:
-            protocol = 'http://'
+            port = 7280
+        protocol = 'http://'
+
+        self.interactive = interactive
 
         h = f"{protocol}{host}:{port}"
-        API.__init__(self, Credentials(h, auth))
+        API.__init__(self, Credentials(h, None))
         if check and self.ping() > 0.5:
             print("warning: connection to this repository may be high latency or unstable.")
 
     def __repr__(self):
         return "Sentenai(host=\"{}\")".format(self._credentials.host)
 
     def __call__(self, tspl):
```

### Comparing `sentenai-1.6.4.5/sentenai/api.py` & `sentenai-1.6.4.6/sentenai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,21 +177,17 @@
         return "Credentials(auth_key='{}', host='{}')".format(
             repr(self.auth_key), self.host)
 
 
 class API(object):
     def __init__(self, credentials, *prefix, params={}):
         self._credentials = credentials
-        if credentials.auth_key:
-            self._session = requests.Session()
-            for auth in credentials.auth_key.items():
-                self._session.auth = auth
-                break
-        else:
-            self._session = requests
+        self._session = requests.Session()
+        a = requests.adapters.HTTPAdapter(pool_connections=100, pool_maxsize=100)
+        self._session.mount('', a)
         self._prefix = prefix
         self._params = params
 
     debug = Debug()
 
     @staticmethod
     def _debug(enable=True):
```

### Comparing `sentenai-1.6.4.5/sentenai/stream/events.py` & `sentenai-1.6.4.6/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.5/sentenai/stream/metadata.py` & `sentenai-1.6.4.6/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.5/sentenai/stream/streams.py` & `sentenai-1.6.4.6/sentenai/stream/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,34 @@
 from queue import Queue
 from threading import Thread
 from concurrent.futures import ThreadPoolExecutor
 
 Update = namedtuple('Update', ['id', 'start', 'end', 'data'])
 
 
-def worker(q, workers, total):
+def worker(q, workers, total, progress, position=None):
     with ThreadPoolExecutor(max_workers=workers) as pool:
-        v = 0
-        with tqdm(total=total, unit=" values") as pbar:
+        if progress:
+            v = 0
+            with tqdm(total=total, unit=" values", position=position) as pbar:
+                while True:
+                    data = q.get()
+                    if not data:
+                        pbar.update(total - v)
+                        break # exit on empty list
+                    list(pool.map(index_data, data))
+                    n = sum([len(v) for d, n, i, v in data])
+                    v += n
+                    pbar.update(n)
+        else:
             while True:
                 data = q.get()
                 if not data:
-                    pbar.update(total - v)
                     break # exit on empty list
                 list(pool.map(index_data, data))
-                n = sum([len(v) for d, n, i, v in data])
-                v += n
-                pbar.update(n)
 
 
 def index_data(args):
     db, node, index, v = args
     counter = 0
     while counter < 10:
         data = cbor2.dumps(v)
@@ -44,15 +51,17 @@
             resp = db._post('nodes', node, 'types', index,
                     json=data, headers={'Content-Type': 'application/cbor'}, raw=True)
         except:
             counter += 1
             sleep(.1)
         else:
             if resp.status_code > 204:
+                resp.close()
                 raise Exception(f"failed on row {i}, column {k}")
+            resp.close()
             break
 
 class WQueue(Queue):
     def write(self, data):
         if data:
             j = {}
             if data.id:
@@ -275,15 +284,15 @@
                 workers = key[-1].stop
                 chunksize = key.step or chunksize
             else:
                 path = key
         elif isinstance(key, slice):
             workers = key.stop
             chunksize = key.step or chunksize
-            path = key.start
+            path = (key.start,)
         else:
             path = (key,)
 
         del self[path]
 
         if content is None:
             nid = self._put('paths', *path, json={'kind': 'directory'})
@@ -351,15 +360,15 @@
                 self._put('nodes', nid, 'types', tmap[cname])
                 cmap[cname] = nid
                 dmap[cname] = []
 
             origin = self.origin
             res = []
             q = Queue()
-            Thread(target=worker, args=(q, workers, len(df) * (len(df.columns) - 1))).start()
+            Thread(target=worker, args=(q, workers, len(df) * (len(df.columns) - 1), self._parent.interactive)).start()
 
             for i, row in df.iterrows():
                 if origin is not None:
                     ts = (row['start'] - origin) // np.timedelta64(1, 'ns')
                 else:
                     ts = row['start'] // np.timedelta64(1, 'ns')
                 try:
```

### Comparing `sentenai-1.6.4.5/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.6/sentenai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.5
+Version: 1.6.4.6
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.5/setup.py` & `sentenai-1.6.4.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.5',
+    version='1.6.4.6',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```


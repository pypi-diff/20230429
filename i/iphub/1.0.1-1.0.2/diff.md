# Comparing `tmp/iphub-1.0.1.tar.gz` & `tmp/iphub-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphub-1.0.1.tar", last modified: Sat Apr 29 09:04:32 2023, max compression
+gzip compressed data, was "iphub-1.0.2.tar", last modified: Sat Apr 29 09:25:44 2023, max compression
```

## Comparing `iphub-1.0.1.tar` & `iphub-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.139773 iphub-1.0.1/
--rw-rw-rw-   0        0        0     1080 2022-03-30 02:32:38.000000 iphub-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 iphub-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      773 2023-04-29 09:04:32.139773 iphub-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-29 09:03:39.000000 iphub-1.0.1/README.MD
-drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.136781 iphub-1.0.1/iphub/
--rw-rw-rw-   0        0        0       44 2022-07-02 12:26:30.000000 iphub-1.0.1/iphub/__init__.py
--rw-rw-rw-   0        0        0     2266 2023-04-29 09:02:47.000000 iphub-1.0.1/iphub/iphub.py
-drwxrwxrwx   0        0        0        0 2023-04-29 09:04:32.138776 iphub-1.0.1/iphub.egg-info/
--rw-rw-rw-   0        0        0      773 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 09:04:32.000000 iphub-1.0.1/iphub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 09:04:32.139773 iphub-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-04-29 09:03:58.000000 iphub-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:25:44.122842 iphub-1.0.2/
+-rw-rw-rw-   0        0        0     1080 2022-03-30 02:32:38.000000 iphub-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 iphub-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      773 2023-04-29 09:25:44.122842 iphub-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-29 09:03:39.000000 iphub-1.0.2/README.MD
+drwxrwxrwx   0        0        0        0 2023-04-29 09:25:44.116869 iphub-1.0.2/iphub/
+-rw-rw-rw-   0        0        0       44 2022-07-02 12:26:30.000000 iphub-1.0.2/iphub/__init__.py
+-rw-rw-rw-   0        0        0     2380 2023-04-29 09:24:52.000000 iphub-1.0.2/iphub/iphub.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:25:44.119847 iphub-1.0.2/iphub.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-04-29 09:25:44.000000 iphub-1.0.2/iphub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-04-29 09:25:44.000000 iphub-1.0.2/iphub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 09:25:44.000000 iphub-1.0.2/iphub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 09:25:44.000000 iphub-1.0.2/iphub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 09:25:44.000000 iphub-1.0.2/iphub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 09:25:44.122842 iphub-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-04-29 09:24:58.000000 iphub-1.0.2/setup.py
```

### Comparing `iphub-1.0.1/LICENSE` & `iphub-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iphub-1.0.1/PKG-INFO` & `iphub-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphub
-Version: 1.0.1
+Version: 1.0.2
 Summary: IPhub.info API wrapper.
 Home-page: https://github.com/DedInc/iphub
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/iphub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `iphub-1.0.1/iphub/iphub.py` & `iphub-1.0.2/iphub/iphub.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,39 @@
             return s
         except:
             raise Exception('Login failed!')
 
     def get_keys(self):
         keys = []
         r = self.session.get('https://iphub.info/account')
+        self.ctoken = r.text.split('token" content="')[1].split('"')[0]
         dem = r.text.split('/apiKey/')
         for line in dem:
             try:
                 if dem.index(line) != 0:
-                    keys.append(line.split('"')[0])
+                    keys.append(line.split('"')[0])                
             except:
-                self.regenerate_key()
-                return self.get_keys()
-        return keys
+                pass
+        if len(keys) == 0:
+            self.generate_key()
+            return self.get_keys()
+        return keys 
 
     def get_key(self, id):
-        try:
-            return 'MT' + self.session.get(f'https://iphub.info/apiKey/{id}').text.split('"MT')[1].split('"')[0]
-        except:
-            return None
+        return self.session.get(f'https://iphub.info/apiKey/{id}').text.split('readonly value="')[1].split('"')[0]
 
     def regenerate_key(self, id):
-        try:
-            self.session.post(f'https://iphub.info/apiKey/regenerateApiKey/{id}', data={'_token': self.ctoken})
-            return self.get_key(id)
-        except:
-            return None
+        r = self.session.post(f'https://iphub.info/apiKey/regenerateApiKey/{id}', data={'_token': self.ctoken})            
+        self.ctoken = r.text.split('token" content="')[1].split('"')[0]
+        return self.get_key(id)
 
     def generate_key(self):
-        try:
-            self.session.post('https://iphub.info/apiKey/newFree', data={'_token': self.ctoken})
-            return self.get_key(self.get_keys()[0])
-        except:
-            return None
+        r = self.session.post('https://iphub.info/apiKey/newFree', data={'_token': self.ctoken})
+        self.ctoken = r.text.split('token" content="')[1].split('"')[0]
+        return self.get_key(self.get_keys()[0])
 
     def check_ip(self, ip):
         r = get(url=f'http://v2.api.iphub.info/ip/{ip}', headers={'X-Key': self.api_key}).json()
         if 'error' in r:
             if '86400' in r['error']:
                 self.set_key(self.regenerate_key(self.get_keys()[0]))
                 return self.check_ip(ip)
```

### Comparing `iphub-1.0.1/iphub.egg-info/PKG-INFO` & `iphub-1.0.2/iphub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphub
-Version: 1.0.1
+Version: 1.0.2
 Summary: IPhub.info API wrapper.
 Home-page: https://github.com/DedInc/iphub
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/iphub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `iphub-1.0.1/setup.py` & `iphub-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='iphub',
-    version='1.0.1',
+    version='1.0.2',
     author='Maehdakvan',
     author_email='visitanimation@google.com',
     description='IPhub.info API wrapper.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DedInc/iphub',
     project_urls={
```


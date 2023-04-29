# Comparing `tmp/zmemory-0.1.0.tar.gz` & `tmp/zmemory-0.1.1.tar.gz`

## Comparing `zmemory-0.1.0.tar` & `zmemory-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 zmemory-0.1.0/src/zmemory/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zmemory-0.1.0/LICENSE
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 zmemory-0.1.0/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zmemory-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 zmemory-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 zmemory-0.1.1/src/zmemory/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zmemory-0.1.1/LICENSE
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 zmemory-0.1.1/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zmemory-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 zmemory-0.1.1/PKG-INFO
```

### Comparing `zmemory-0.1.0/src/zmemory/__init__.py` & `zmemory-0.1.1/src/zmemory/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from redis import Redis
+import json
 
 
 class Memory(object):
     def __init__(self, config):
         self.instance = Redis(decode_responses=True, **config)
 
     def get(self, k):
         """获取值
         c.get('access_token_00b73bbe23f34a468b2a5f158701f17f_wx')
         """
-        return self.instance.get(k)
+        v = self.instance.get(k)
+        return json.loads(v)
 
-    def set(self, k, v, *args):
+    def set(self, k, v, seconds=0):
         """修改值
         c.get('access_token_00b73bbe23f34a468b2a5f158701f17f_wx')
         """
-        return self.instance.set(k, v, *args)
+        v = json.dumps(v, ensure_ascii=False)
+        self.instance.set(k, v)
+        self.expire(k, seconds)
 
     def hget(self, name, k):
         """获取值
         c.get('access_token_00b73bbe23f34a468b2a5f158701f17f_wx')
         """
         return self.instance.hget(name, k)
```

### Comparing `zmemory-0.1.0/LICENSE` & `zmemory-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zmemory-0.1.0/pyproject.toml` & `zmemory-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zmemory"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen memory library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zmemory-0.1.0/PKG-INFO` & `zmemory-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zmemory
-Version: 0.1.0
+Version: 0.1.1
 Summary: zen memory library
 Project-URL: Homepage, https://github.com/inspirare6/zmemory
 Project-URL: Bug Tracker, https://github.com/inspirare6/zmemory/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/betterconfigs-0.7-py3-none-any.whl.zip` & `tmp/betterconfigs-0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14841 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2772 b- defN 20-Feb-02 00:00 betterconfigs/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 20-Feb-02 00:00 betterconfigs/utilities.py
-?rw-r--r--  2.0 unx     1413 b- defN 20-Feb-02 00:00 betterconfigs-0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 betterconfigs-0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35148 b- defN 20-Feb-02 00:00 betterconfigs-0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      484 b- defN 20-Feb-02 00:00 betterconfigs-0.7.dist-info/RECORD
-6 files, 40124 bytes uncompressed, 13967 bytes compressed:  65.2%
+Zip file size: 15552 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4810 b- defN 20-Feb-02 00:00 betterconfigs/__init__.py
+-rw-r--r--  2.0 unx      323 b- defN 20-Feb-02 00:00 betterconfigs/utilities.py
+?rw-r--r--  2.0 unx     2278 b- defN 20-Feb-02 00:00 betterconfigs-0.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 betterconfigs-0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35148 b- defN 20-Feb-02 00:00 betterconfigs-0.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      484 b- defN 20-Feb-02 00:00 betterconfigs-0.8.dist-info/RECORD
+6 files, 43130 bytes uncompressed, 14678 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: betterconfigs/__init__.py
 Comment: 
 
 Filename: betterconfigs/utilities.py
 Comment: 
 
-Filename: betterconfigs-0.7.dist-info/METADATA
+Filename: betterconfigs-0.8.dist-info/METADATA
 Comment: 
 
-Filename: betterconfigs-0.7.dist-info/WHEEL
+Filename: betterconfigs-0.8.dist-info/WHEEL
 Comment: 
 
-Filename: betterconfigs-0.7.dist-info/licenses/LICENSE
+Filename: betterconfigs-0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: betterconfigs-0.7.dist-info/RECORD
+Filename: betterconfigs-0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## betterconfigs/__init__.py

```diff
@@ -1,51 +1,59 @@
 import pickle
 import os
 import warnings
-executableVersion = "0.7"
+from cryptography.fernet import Fernet
+executableVersion = "0.8"
 class config:
     def __init__(self, path) -> None:
         self.path = path
+        self.encKey = None
         if os.path.exists(path)==False:
             try:
                 loadConfig = {}
                 loadConfig['_version'] = executableVersion
+                loadConfig['_encrypted'] = False
+                self.encKey = Fernet.generate_key()
                 with open(self.path, 'wb') as handle:
                     pickle.dump(loadConfig, handle, protocol=pickle.HIGHEST_PROTOCOL)
             except:
                 raise Exception("attempted to initialize the configuration file but was unable to write")
     def __getitem__(self, key):
         self.checkReady()
         try:
+            if self.getRaw('_encrypted'):
+                return self.decryptValue(key)
             with open(self.path, 'rb') as handle:
                 loadedConfig = pickle.load(handle)
             return loadedConfig[key]
         except FileNotFoundError:
             raise Exception("configuration might not be initialized")
         except:
             raise NameError("property doesn't exist in configuration")
     def __setitem__(self, key, value):
         self.checkReady()
-        if key == '_version':
-            raise Exception("unable to change configuration version")
+        if key.startswith('_'):
+            raise Exception("unable to change configuration property")
         try:
+            if self.getRaw('_encrypted'):
+                value = self.encryptValue(value)
             with open(self.path, 'rb') as handle:
                 loadedConfig = pickle.load(handle)
             loadedConfig[key] = value
             with open(self.path, 'wb') as handle:
                 pickle.dump(loadedConfig, handle, protocol=pickle.HIGHEST_PROTOCOL)
             return 0
         except FileExistsError:
             raise Exception("unable to find the configuration")
         except:
             raise Exception("error writing configuration file")
     def __delitem__(self, key):
         self.checkReady()
-        if key == '_version':
-            raise Exception("unable to delete configuration version")
+        if key.startswith('_'):
+            raise Exception("unable to delete configuration property")
         try:
             with open(self.path, 'rb') as handle:
                 loadedConfig = pickle.load(handle)
             loadedConfig.pop(key)
             with open(self.path, 'wb') as handle:
                 pickle.dump(loadedConfig, handle, protocol=pickle.HIGHEST_PROTOCOL)
             return 0
@@ -59,9 +67,49 @@
                 loadedConfig = pickle.load(handle)
             return loadedConfig[key]
         except FileNotFoundError:
             raise Exception("configuration might not be initialized")
         except:
             raise NameError("property doesn't exist in configuration")
     def checkReady(self):
+        if self.encKey==None and self.getRaw('_encrypted')==True:
+            raise Exception('configuration is marked encrypted, but no encKey provided')
         if self.getRaw('_version')!=executableVersion:
             warnings.warn("version mismatch!")
+    def checkEncryptionValidity(self):
+        self.checkReady()
+        if self.decryptValue('_checksum')==self.encKey.decode():
+            return 0
+        else:
+            return 1
+    def encryptValue(self, value):
+        self.checkReady()
+        fernet = Fernet(self.encKey)
+        return fernet.encrypt(value.encode())
+    def decryptValue(self, key):
+        self.checkReady()
+        fernet = Fernet(self.encKey)
+        return fernet.decrypt(self.getRaw(key)).decode()
+    def encryptFile(self):
+        self.checkReady()
+        with open(self.path, 'rb') as handle:
+                loadedConfig = pickle.load(handle)
+        for i in loadedConfig:
+            if not i.startswith("_"):
+                loadedConfig[i] = self.encryptValue(loadedConfig[i])
+        loadedConfig['_encrypted']=True
+        loadedConfig['_checksum']=self.encryptValue(self.encKey.decode())
+        with open(self.path, 'wb') as handle:
+                pickle.dump(loadedConfig, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        return 0
+    def decryptFile(self):
+        self.checkReady()
+        with open(self.path, 'rb') as handle:
+                loadedConfig = pickle.load(handle)
+        for i in loadedConfig:
+            if not i.startswith("_"):
+                loadedConfig[i] = self.decryptValue(i)
+        loadedConfig['_encrypted']=False
+        loadedConfig.pop('_checksum')
+        with open(self.path, 'wb') as handle:
+                pickle.dump(loadedConfig, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        return 0
```

## betterconfigs/utilities.py

```diff
@@ -1,8 +1,10 @@
 import pickle
-import os
-import warnings
-from __init__ import executableVersion
 def ls(path):
     with open(path, 'rb') as handle:
         loadedConfig = pickle.load(handle)
-    print("Version: ",loadedConfig['_version'])
+    print("Version: ",loadedConfig['_version'])
+    print("Encrypted: ", loadedConfig['_encrypted'])
+    try:
+        print("Checksum: ", loadedConfig['_checksum'])
+    except:
+        print("No checksum available")
```

## Comparing `betterconfigs-0.7.dist-info/licenses/LICENSE` & `betterconfigs-0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*


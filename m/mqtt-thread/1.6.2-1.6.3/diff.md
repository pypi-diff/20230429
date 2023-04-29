# Comparing `tmp/mqtt_thread-1.6.2.tar.gz` & `tmp/mqtt_thread-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_thread-1.6.2.tar", last modified: Sat Apr 15 21:21:30 2023, max compression
+gzip compressed data, was "mqtt_thread-1.6.3.tar", last modified: Sat Apr 29 17:04:48 2023, max compression
```

## Comparing `mqtt_thread-1.6.2.tar` & `mqtt_thread-1.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 21:21:30.259375 mqtt_thread-1.6.2/
--rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.2/LICENCE
--rw-rw-rw-   0        0        0     3720 2023-04-15 21:21:30.259375 mqtt_thread-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 21:21:30.243737 mqtt_thread-1.6.2/mqtt_thread/
--rw-rw-rw-   0        0        0     7276 2023-04-15 21:20:36.000000 mqtt_thread-1.6.2/mqtt_thread/MQTT_Thread.py
--rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.2/mqtt_thread/MQTT_Thread_bak.py
--rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.2/mqtt_thread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 21:21:30.259375 mqtt_thread-1.6.2/mqtt_thread.egg-info/
--rw-rw-rw-   0        0        0     3720 2023-04-15 21:21:30.000000 mqtt_thread-1.6.2/mqtt_thread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-04-15 21:21:30.000000 mqtt_thread-1.6.2/mqtt_thread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 21:21:30.000000 mqtt_thread-1.6.2/mqtt_thread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 21:21:30.000000 mqtt_thread-1.6.2/mqtt_thread.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 21:21:30.000000 mqtt_thread-1.6.2/mqtt_thread.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 21:21:30.259375 mqtt_thread-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-04-15 21:20:53.000000 mqtt_thread-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:04:48.824964 mqtt_thread-1.6.3/
+-rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.3/LICENCE
+-rw-rw-rw-   0        0        0     3720 2023-04-29 17:04:48.824964 mqtt_thread-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:04:48.824964 mqtt_thread-1.6.3/mqtt_thread/
+-rw-rw-rw-   0        0        0     7430 2023-04-29 17:02:46.000000 mqtt_thread-1.6.3/mqtt_thread/MQTT_Thread.py
+-rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.3/mqtt_thread/MQTT_Thread_bak.py
+-rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.3/mqtt_thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:04:48.824964 mqtt_thread-1.6.3/mqtt_thread.egg-info/
+-rw-rw-rw-   0        0        0     3720 2023-04-29 17:04:48.000000 mqtt_thread-1.6.3/mqtt_thread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-29 17:04:48.000000 mqtt_thread-1.6.3/mqtt_thread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:04:48.000000 mqtt_thread-1.6.3/mqtt_thread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 17:04:48.000000 mqtt_thread-1.6.3/mqtt_thread.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 17:04:48.000000 mqtt_thread-1.6.3/mqtt_thread.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:04:48.840592 mqtt_thread-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-04-29 17:03:20.000000 mqtt_thread-1.6.3/setup.py
```

### Comparing `mqtt_thread-1.6.2/LICENCE` & `mqtt_thread-1.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.2/PKG-INFO` & `mqtt_thread-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt_thread
-Version: 1.6.2
+Version: 1.6.3
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.2/README.md` & `mqtt_thread-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.2/mqtt_thread/MQTT_Thread.py` & `mqtt_thread-1.6.3/mqtt_thread/MQTT_Thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,12 @@
         self.nomFichier = nomFic
 
     def Record(self,val):
         self.record = val
 
     def messageArrived(self):# fonction vide à personnaliser.... dans l'instance.
         pass
+
+    def stop(self):
+        print('La connexion MQTT est fermée.')
+        self.client.disconnect()
+        print('Le thread va être arrêté !')
```

### Comparing `mqtt_thread-1.6.2/mqtt_thread/MQTT_Thread_bak.py` & `mqtt_thread-1.6.3/mqtt_thread/MQTT_Thread_bak.py`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.2/mqtt_thread.egg-info/PKG-INFO` & `mqtt_thread-1.6.3/mqtt_thread.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-thread
-Version: 1.6.2
+Version: 1.6.3
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.2/setup.py` & `mqtt_thread-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqtt_thread", # Replace with your own username
-    version="1.6.2",
+    version="1.6.3",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connection MQTT with thread",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```


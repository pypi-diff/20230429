# Comparing `tmp/circular_queue-0.0.1.tar.gz` & `tmp/circular_queue-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular_queue-0.0.1.tar", last modified: Sat Apr 29 20:52:51 2023, max compression
+gzip compressed data, was "circular_queue-0.0.2.tar", last modified: Sat Apr 29 21:13:05 2023, max compression
```

## Comparing `circular_queue-0.0.1.tar` & `circular_queue-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 20:52:51.570249 circular_queue-0.0.1/
--rw-r--r--   0 kiwiair    (501) staff       (20)     1063 2023-04-29 16:01:30.000000 circular_queue-0.0.1/LICENSE.md
--rw-r--r--   0 kiwiair    (501) staff       (20)     2037 2023-04-29 20:52:51.569786 circular_queue-0.0.1/PKG-INFO
--rw-r--r--   0 kiwiair    (501) staff       (20)     1505 2023-04-29 20:40:48.000000 circular_queue-0.0.1/README.md
--rw-r--r--   0 kiwiair    (501) staff       (20)      601 2023-04-29 20:52:35.000000 circular_queue-0.0.1/pyproject.toml
--rw-r--r--   0 kiwiair    (501) staff       (20)       38 2023-04-29 20:52:51.570373 circular_queue-0.0.1/setup.cfg
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 20:52:51.567573 circular_queue-0.0.1/src/
--rw-r--r--   0 kiwiair    (501) staff       (20)        0 2022-02-15 23:10:08.000000 circular_queue-0.0.1/src/__init__.py
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 20:52:51.568988 circular_queue-0.0.1/src/circular_queue.egg-info/
--rw-r--r--   0 kiwiair    (501) staff       (20)     2037 2023-04-29 20:52:51.000000 circular_queue-0.0.1/src/circular_queue.egg-info/PKG-INFO
--rw-r--r--   0 kiwiair    (501) staff       (20)      270 2023-04-29 20:52:51.000000 circular_queue-0.0.1/src/circular_queue.egg-info/SOURCES.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)        1 2023-04-29 20:52:51.000000 circular_queue-0.0.1/src/circular_queue.egg-info/dependency_links.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)       24 2023-04-29 20:52:51.000000 circular_queue-0.0.1/src/circular_queue.egg-info/top_level.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)     1916 2022-02-23 20:51:22.000000 circular_queue-0.0.1/src/circular_queue.py
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 20:52:51.569355 circular_queue-0.0.1/tests/
--rw-r--r--   0 kiwiair    (501) staff       (20)     3036 2023-04-29 20:39:44.000000 circular_queue-0.0.1/tests/test_circular_queue.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.292709 circular_queue-0.0.2/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1063 2023-04-29 16:01:30.000000 circular_queue-0.0.2/LICENSE.md
+-rw-r--r--   0 kiwiair    (501) staff       (20)     2009 2023-04-29 21:13:05.292430 circular_queue-0.0.2/PKG-INFO
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1477 2023-04-29 21:08:17.000000 circular_queue-0.0.2/README.md
+-rw-r--r--   0 kiwiair    (501) staff       (20)      601 2023-04-29 21:12:51.000000 circular_queue-0.0.2/pyproject.toml
+-rw-r--r--   0 kiwiair    (501) staff       (20)       38 2023-04-29 21:13:05.292791 circular_queue-0.0.2/setup.cfg
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.290641 circular_queue-0.0.2/src/
+-rw-r--r--   0 kiwiair    (501) staff       (20)        0 2022-02-15 23:10:08.000000 circular_queue-0.0.2/src/__init__.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.291700 circular_queue-0.0.2/src/circular_queue.egg-info/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     2009 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/PKG-INFO
+-rw-r--r--   0 kiwiair    (501) staff       (20)      270 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)        1 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)       24 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/top_level.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1916 2022-02-23 20:51:22.000000 circular_queue-0.0.2/src/circular_queue.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.291961 circular_queue-0.0.2/tests/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     3036 2023-04-29 20:39:44.000000 circular_queue-0.0.2/tests/test_circular_queue.py
```

### Comparing `circular_queue-0.0.1/LICENSE.md` & `circular_queue-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `circular_queue-0.0.1/PKG-INFO` & `circular_queue-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular_queue
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pythonic implementation of a circular queue
 Author-email: Gui Luz <salgl@yahoo.com.br>
 Project-URL: Homepage, https://github.com/Gui-Luz/circular-queue
 Project-URL: Bug Tracker, https://github.com/Gui-Luz/circular-queue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # Circular Queue
 ### A pythonic implementation of the beloved data structure
 Circular Queue is an object that can be used whenever you need to connect the head of an iterable to its tail. 
 It can be easily connected to a database in order to persist your queue rotation.  
 ##### Installation
 ```
-git clone https://github.com/Gui-Luz/CircularQueue.git
+pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
 from CircularQueue.circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
```

### Comparing `circular_queue-0.0.1/README.md` & `circular_queue-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Circular Queue
 ### A pythonic implementation of the beloved data structure
 Circular Queue is an object that can be used whenever you need to connect the head of an iterable to its tail. 
 It can be easily connected to a database in order to persist your queue rotation.  
 ##### Installation
 ```
-git clone https://github.com/Gui-Luz/CircularQueue.git
+pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
 from CircularQueue.circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
```

### Comparing `circular_queue-0.0.1/pyproject.toml` & `circular_queue-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "circular_queue"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gui Luz", email="salgl@yahoo.com.br" },
 ]
 description = "A pythonic implementation of a circular queue"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `circular_queue-0.0.1/src/circular_queue.egg-info/PKG-INFO` & `circular_queue-0.0.2/src/circular_queue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-queue
-Version: 0.0.1
+Version: 0.0.2
 Summary: A pythonic implementation of a circular queue
 Author-email: Gui Luz <salgl@yahoo.com.br>
 Project-URL: Homepage, https://github.com/Gui-Luz/circular-queue
 Project-URL: Bug Tracker, https://github.com/Gui-Luz/circular-queue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # Circular Queue
 ### A pythonic implementation of the beloved data structure
 Circular Queue is an object that can be used whenever you need to connect the head of an iterable to its tail. 
 It can be easily connected to a database in order to persist your queue rotation.  
 ##### Installation
 ```
-git clone https://github.com/Gui-Luz/CircularQueue.git
+pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
 from CircularQueue.circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
```

### Comparing `circular_queue-0.0.1/src/circular_queue.py` & `circular_queue-0.0.2/src/circular_queue.py`

 * *Files identical despite different names*

### Comparing `circular_queue-0.0.1/tests/test_circular_queue.py` & `circular_queue-0.0.2/tests/test_circular_queue.py`

 * *Files identical despite different names*


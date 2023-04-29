# Comparing `tmp/circular_queue-0.0.2.tar.gz` & `tmp/circular_queue-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular_queue-0.0.2.tar", last modified: Sat Apr 29 21:13:05 2023, max compression
+gzip compressed data, was "circular_queue-0.0.3.tar", last modified: Sat Apr 29 21:19:26 2023, max compression
```

## Comparing `circular_queue-0.0.2.tar` & `circular_queue-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.292709 circular_queue-0.0.2/
--rw-r--r--   0 kiwiair    (501) staff       (20)     1063 2023-04-29 16:01:30.000000 circular_queue-0.0.2/LICENSE.md
--rw-r--r--   0 kiwiair    (501) staff       (20)     2009 2023-04-29 21:13:05.292430 circular_queue-0.0.2/PKG-INFO
--rw-r--r--   0 kiwiair    (501) staff       (20)     1477 2023-04-29 21:08:17.000000 circular_queue-0.0.2/README.md
--rw-r--r--   0 kiwiair    (501) staff       (20)      601 2023-04-29 21:12:51.000000 circular_queue-0.0.2/pyproject.toml
--rw-r--r--   0 kiwiair    (501) staff       (20)       38 2023-04-29 21:13:05.292791 circular_queue-0.0.2/setup.cfg
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.290641 circular_queue-0.0.2/src/
--rw-r--r--   0 kiwiair    (501) staff       (20)        0 2022-02-15 23:10:08.000000 circular_queue-0.0.2/src/__init__.py
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.291700 circular_queue-0.0.2/src/circular_queue.egg-info/
--rw-r--r--   0 kiwiair    (501) staff       (20)     2009 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/PKG-INFO
--rw-r--r--   0 kiwiair    (501) staff       (20)      270 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/SOURCES.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)        1 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/dependency_links.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)       24 2023-04-29 21:13:05.000000 circular_queue-0.0.2/src/circular_queue.egg-info/top_level.txt
--rw-r--r--   0 kiwiair    (501) staff       (20)     1916 2022-02-23 20:51:22.000000 circular_queue-0.0.2/src/circular_queue.py
-drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:13:05.291961 circular_queue-0.0.2/tests/
--rw-r--r--   0 kiwiair    (501) staff       (20)     3036 2023-04-29 20:39:44.000000 circular_queue-0.0.2/tests/test_circular_queue.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:19:26.078475 circular_queue-0.0.3/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1063 2023-04-29 16:01:30.000000 circular_queue-0.0.3/LICENSE.md
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1995 2023-04-29 21:19:26.078116 circular_queue-0.0.3/PKG-INFO
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1463 2023-04-29 21:18:17.000000 circular_queue-0.0.3/README.md
+-rw-r--r--   0 kiwiair    (501) staff       (20)      601 2023-04-29 21:18:17.000000 circular_queue-0.0.3/pyproject.toml
+-rw-r--r--   0 kiwiair    (501) staff       (20)       38 2023-04-29 21:19:26.078581 circular_queue-0.0.3/setup.cfg
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:19:26.076101 circular_queue-0.0.3/src/
+-rw-r--r--   0 kiwiair    (501) staff       (20)        0 2022-02-15 23:10:08.000000 circular_queue-0.0.3/src/__init__.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:19:26.077337 circular_queue-0.0.3/src/circular_queue.egg-info/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1995 2023-04-29 21:19:26.000000 circular_queue-0.0.3/src/circular_queue.egg-info/PKG-INFO
+-rw-r--r--   0 kiwiair    (501) staff       (20)      270 2023-04-29 21:19:26.000000 circular_queue-0.0.3/src/circular_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)        1 2023-04-29 21:19:26.000000 circular_queue-0.0.3/src/circular_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)       24 2023-04-29 21:19:26.000000 circular_queue-0.0.3/src/circular_queue.egg-info/top_level.txt
+-rw-r--r--   0 kiwiair    (501) staff       (20)     1916 2022-02-23 20:51:22.000000 circular_queue-0.0.3/src/circular_queue.py
+drwxr-xr-x   0 kiwiair    (501) staff       (20)        0 2023-04-29 21:19:26.077713 circular_queue-0.0.3/tests/
+-rw-r--r--   0 kiwiair    (501) staff       (20)     3036 2023-04-29 20:39:44.000000 circular_queue-0.0.3/tests/test_circular_queue.py
```

### Comparing `circular_queue-0.0.2/LICENSE.md` & `circular_queue-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `circular_queue-0.0.2/PKG-INFO` & `circular_queue-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular_queue
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pythonic implementation of a circular queue
 Author-email: Gui Luz <salgl@yahoo.com.br>
 Project-URL: Homepage, https://github.com/Gui-Luz/circular-queue
 Project-URL: Bug Tracker, https://github.com/Gui-Luz/circular-queue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 ##### Installation
 ```
 pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
-from CircularQueue.circular_queue import CircularQueue
+from circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
 ```python3
 mylist = ['Banana', 'Star Fruit', 'Apple', 'Orange', 'Avocado']
 pointer = 'Apple'
 myqueue = CircularQueue(mylist, pointer)
 ```
```

### Comparing `circular_queue-0.0.2/README.md` & `circular_queue-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ##### Installation
 ```
 pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
-from CircularQueue.circular_queue import CircularQueue
+from circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
 ```python3
 mylist = ['Banana', 'Star Fruit', 'Apple', 'Orange', 'Avocado']
 pointer = 'Apple'
 myqueue = CircularQueue(mylist, pointer)
 ```
```

### Comparing `circular_queue-0.0.2/pyproject.toml` & `circular_queue-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "circular_queue"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gui Luz", email="salgl@yahoo.com.br" },
 ]
 description = "A pythonic implementation of a circular queue"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `circular_queue-0.0.2/src/circular_queue.egg-info/PKG-INFO` & `circular_queue-0.0.3/src/circular_queue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-queue
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pythonic implementation of a circular queue
 Author-email: Gui Luz <salgl@yahoo.com.br>
 Project-URL: Homepage, https://github.com/Gui-Luz/circular-queue
 Project-URL: Bug Tracker, https://github.com/Gui-Luz/circular-queue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 ##### Installation
 ```
 pip install circular-queue
 ```
 ##### How to use
 After cloning the repo, you can import the **CircularQueue** class to your project:
 ```python3
-from CircularQueue.circular_queue import CircularQueue
+from circular_queue import CircularQueue
 ```
 You can instantiate the **CircularQueue** object passing a **queue** an a **pointer** as arguments:
 ```python3
 mylist = ['Banana', 'Star Fruit', 'Apple', 'Orange', 'Avocado']
 pointer = 'Apple'
 myqueue = CircularQueue(mylist, pointer)
 ```
```

### Comparing `circular_queue-0.0.2/src/circular_queue.py` & `circular_queue-0.0.3/src/circular_queue.py`

 * *Files identical despite different names*

### Comparing `circular_queue-0.0.2/tests/test_circular_queue.py` & `circular_queue-0.0.3/tests/test_circular_queue.py`

 * *Files identical despite different names*


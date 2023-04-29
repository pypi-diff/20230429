# Comparing `tmp/ooze-0.1.2.tar.gz` & `tmp/ooze-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooze-0.1.2.tar", last modified: Tue Sep 13 21:15:40 2022, max compression
+gzip compressed data, was "ooze-1.0.0.tar", last modified: Fri Apr 28 23:57:21 2023, max compression
```

## Comparing `ooze-0.1.2.tar` & `ooze-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:15:40.435809 ooze-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-13 21:15:12.000000 ooze-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    42502 2022-09-13 21:15:40.435809 ooze-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-09-13 21:15:12.000000 ooze-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:15:40.435809 ooze-0.1.2/ooze/
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-09-13 21:15:12.000000 ooze-0.1.2/ooze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-09-13 21:15:12.000000 ooze-0.1.2/ooze/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:15:40.435809 ooze-0.1.2/ooze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    42502 2022-09-13 21:15:40.000000 ooze-0.1.2/ooze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-13 21:15:40.000000 ooze-0.1.2/ooze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 21:15:40.000000 ooze-0.1.2/ooze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-13 21:15:40.000000 ooze-0.1.2/ooze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-13 21:15:40.000000 ooze-0.1.2/ooze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-09-13 21:15:12.000000 ooze-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-13 21:15:40.435809 ooze-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-13 21:15:12.000000 ooze-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 23:56:58.000000 ooze-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-04-28 23:57:21.611228 ooze-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 23:56:58.000000 ooze-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.607228 ooze-1.0.0/ooze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-28 23:56:58.000000 ooze-1.0.0/ooze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 23:56:58.000000 ooze-1.0.0/ooze/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/ooze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-28 23:56:58.000000 ooze-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 23:57:21.611228 ooze-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 23:56:58.000000 ooze-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-28 23:56:58.000000 ooze-1.0.0/tests/test_ooze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-28 23:56:58.000000 ooze-1.0.0/tests/test_pool.py
```

### Comparing `ooze-0.1.2/LICENSE` & `ooze-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ooze-0.1.2/PKG-INFO` & `ooze-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooze
-Version: 0.1.2
+Version: 1.0.0
 Summary: Brain-dead simple dependency injection
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooze-0.1.2/README.md` & `ooze-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ooze-0.1.2/ooze/__init__.py` & `ooze-1.0.0/ooze/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         return class_to_provide
     elif inspect.isfunction(name_or_item):
         func_to_provide = name_or_item
         func_name = name_or_item.__name__.lower()
         _INSTANCES[func_name] = func_to_provide
         return func_to_provide
     else:
+        @functools.wraps(name_or_item)
         def inner_provide(item):
             name = name_or_item.lower()
             if inspect.isclass(item):
                 _CLASSES_TO_INSTANTIATE[name] = item
             else:
                 _INSTANCES[name] = item
             return item
@@ -166,14 +167,15 @@
     """A decorator to add a factory to the dependency graph."""
     if callable(name_or_item):
         factory_func = name_or_item
         factory_name = factory_func.__name__.lower()
         _FACTORIES[factory_name] = factory_func
         return factory_func
     else:
+        @functools.wraps(name_or_item)
         def inner_factory(item):
             inner_factory_func = item
             inner_factory_name = name_or_item
             _FACTORIES[inner_factory_name] = inner_factory_func
             return inner_factory_func
 
         return inner_factory
```

### Comparing `ooze-0.1.2/ooze.egg-info/PKG-INFO` & `ooze-1.0.0/ooze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooze
-Version: 0.1.2
+Version: 1.0.0
 Summary: Brain-dead simple dependency injection
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooze-0.1.2/pyproject.toml` & `ooze-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooze"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name="Steve Brettschneider", email="steve@bluehousefamily.com" },
 ]
 description = "Brain-dead simple dependency injection"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```


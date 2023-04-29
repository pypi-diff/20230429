# Comparing `tmp/portabletab-0.3.1.tar.gz` & `tmp/portabletab-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portabletab-0.3.1.tar", max compression
+gzip compressed data, was "portabletab-0.3.2.tar", max compression
```

## Comparing `portabletab-0.3.1.tar` & `portabletab-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.1/LICENSE
--rw-r--r--   0        0        0      203 2023-04-11 03:07:38.494545 portabletab-0.3.1/PortableTab/__init__.py
--rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.1/PortableTab/__main__.py
--rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.1/PortableTab/base_table.py
--rw-r--r--   0        0        0     4673 2023-04-04 07:41:11.567861 portabletab-0.3.1/PortableTab/capnp_manager.py
--rw-r--r--   0        0        0    18355 2023-04-11 03:07:38.498545 portabletab-0.3.1/PortableTab/capnp_table.py
--rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.1/PortableTab/exceptions.py
--rw-r--r--   0        0        0     1837 2023-04-11 03:07:29.170336 portabletab-0.3.1/README.md
--rw-r--r--   0        0        0      634 2023-04-11 03:07:38.498545 portabletab-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-01 08:14:02.000000 portabletab-0.3.2/LICENSE
+-rw-r--r--   0        0        0      203 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/__init__.py
+-rw-r--r--   0        0        0     4861 2023-04-29 09:02:43.908411 portabletab-0.3.2/PortableTab/__main__.py
+-rw-r--r--   0        0        0     1917 2023-04-05 12:03:54.000000 portabletab-0.3.2/PortableTab/base_table.py
+-rw-r--r--   0        0        0     4697 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/capnp_manager.py
+-rw-r--r--   0        0        0    18486 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/capnp_table.py
+-rw-r--r--   0        0        0      155 2023-04-29 09:02:43.908411 portabletab-0.3.2/PortableTab/exceptions.py
+-rw-r--r--   0        0        0     1837 2023-04-09 02:51:51.000000 portabletab-0.3.2/README.md
+-rw-r--r--   0        0        0      634 2023-04-29 09:02:48.188411 portabletab-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 portabletab-0.3.2/setup.py
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.2/PKG-INFO
```

### Comparing `portabletab-0.3.1/LICENSE` & `portabletab-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.1/PortableTab/__main__.py` & `portabletab-0.3.2/PortableTab/__main__.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.1/PortableTab/base_table.py` & `portabletab-0.3.2/PortableTab/base_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.1/PortableTab/capnp_manager.py` & `portabletab-0.3.2/PortableTab/capnp_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,20 +133,22 @@
         Unload capnp schema from the name space.
 
         Parameters
         ----------
         names: [str], optional
             List of assigned names for the modules to be unloaded.
         """
+        new_modules = {}
         for name, module in cls.modules.items():
             if names is None or name in names:
-                cls.modules[name] = None
                 del module
+            else:
+                new_modules[name] = cls.modules[name]
 
-        cls.modules = {n: m for n, m in cls.modules.items() if m}
+        cls.modules = new_modules
 
     def get_page_mmap(self, page_path: Path) -> mmap.mmap:
         """
         Get mmap object assigned to the page file.
 
         Parameters
         ----------
```

### Comparing `portabletab-0.3.1/PortableTab/capnp_table.py` & `portabletab-0.3.2/PortableTab/capnp_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         Notes
         -----
         - This method is automatically called when needed.
           There is no need to call it explicitly from the user program.
         """
         config = self.get_config()
         module_name = config["module_name"]
+        logger.debug(f"module_name: '{module_name}")
         if module_name not in CapnpManager.modules:
+            logger.debug(f"{module_name} is not in modules, loading schema.")
             CapnpManager.load_schema(
                 self.get_dir() / config["capnp_file"],
                 module_name)
 
     @lru_cache(maxsize=128)
     def get_record_type(self) -> Any:
         """
```

### Comparing `portabletab-0.3.1/README.md` & `portabletab-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.1/PKG-INFO` & `portabletab-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portabletab
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python package for serializing tables in portable format with Capnp.
 License: MIT
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


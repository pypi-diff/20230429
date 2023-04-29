# Comparing `tmp/flopsy-0.0.1.tar.gz` & `tmp/flopsy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flopsy-0.0.1.tar", last modified: Sun Apr 23 19:06:29 2023, max compression
+gzip compressed data, was "flopsy-0.0.2.tar", last modified: Sat Apr 29 14:31:11 2023, max compression
```

## Comparing `flopsy-0.0.1.tar` & `flopsy-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-23 19:06:29.179154 flopsy-0.0.1/
--rw-r--r--   0 grib      (1000) grib      (1000)     1077 2023-04-20 16:24:01.000000 flopsy-0.0.1/LICENSE.txt
--rw-r--r--   0 grib      (1000) grib      (1000)      562 2023-04-23 19:06:29.179154 flopsy-0.0.1/PKG-INFO
--rw-r--r--   0 grib      (1000) grib      (1000)     4614 2023-04-23 16:16:02.000000 flopsy-0.0.1/README.md
-drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-23 19:06:29.179154 flopsy-0.0.1/flopsy/
--rw-r--r--   0 grib      (1000) grib      (1000)        0 2023-04-18 20:44:37.000000 flopsy-0.0.1/flopsy/__init__.py
--rw-r--r--   0 grib      (1000) grib      (1000)      316 2023-04-17 22:17:00.000000 flopsy-0.0.1/flopsy/action.py
-drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-23 19:06:29.179154 flopsy-0.0.1/flopsy/inspector/
--rw-r--r--   0 grib      (1000) grib      (1000)    10305 2023-04-23 18:55:45.000000 flopsy-0.0.1/flopsy/inspector/inspector.py
--rw-r--r--   0 grib      (1000) grib      (1000)     2011 2023-04-22 20:00:32.000000 flopsy-0.0.1/flopsy/reducer.py
--rw-r--r--   0 grib      (1000) grib      (1000)     1978 2023-04-22 20:01:20.000000 flopsy-0.0.1/flopsy/saga.py
--rw-r--r--   0 grib      (1000) grib      (1000)     7366 2023-04-23 15:35:23.000000 flopsy-0.0.1/flopsy/store.py
--rw-r--r--   0 grib      (1000) grib      (1000)     1102 2023-04-22 20:21:56.000000 flopsy-0.0.1/flopsy/testapp.py
-drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-23 19:06:29.179154 flopsy-0.0.1/flopsy.egg-info/
--rw-r--r--   0 grib      (1000) grib      (1000)      562 2023-04-23 19:06:29.000000 flopsy-0.0.1/flopsy.egg-info/PKG-INFO
--rw-r--r--   0 grib      (1000) grib      (1000)      322 2023-04-23 19:06:29.000000 flopsy-0.0.1/flopsy.egg-info/SOURCES.txt
--rw-r--r--   0 grib      (1000) grib      (1000)        1 2023-04-23 19:06:29.000000 flopsy-0.0.1/flopsy.egg-info/dependency_links.txt
--rw-r--r--   0 grib      (1000) grib      (1000)       26 2023-04-23 19:06:29.000000 flopsy-0.0.1/flopsy.egg-info/requires.txt
--rw-r--r--   0 grib      (1000) grib      (1000)        7 2023-04-23 19:06:29.000000 flopsy-0.0.1/flopsy.egg-info/top_level.txt
--rw-r--r--   0 grib      (1000) grib      (1000)       79 2023-04-23 19:06:29.179154 flopsy-0.0.1/setup.cfg
--rw-r--r--   0 grib      (1000) grib      (1000)      795 2023-04-23 19:05:30.000000 flopsy-0.0.1/setup.py
+drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-29 14:31:11.929724 flopsy-0.0.2/
+-rw-r--r--   0 grib      (1000) grib      (1000)     1077 2023-04-20 16:24:01.000000 flopsy-0.0.2/LICENSE.txt
+-rw-r--r--   0 grib      (1000) grib      (1000)      562 2023-04-29 14:31:11.929724 flopsy-0.0.2/PKG-INFO
+-rw-r--r--   0 grib      (1000) grib      (1000)     4614 2023-04-23 16:16:02.000000 flopsy-0.0.2/README.md
+drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-29 14:31:11.925724 flopsy-0.0.2/flopsy/
+-rw-r--r--   0 grib      (1000) grib      (1000)        0 2023-04-18 20:44:37.000000 flopsy-0.0.2/flopsy/__init__.py
+-rw-r--r--   0 grib      (1000) grib      (1000)      316 2023-04-17 22:17:00.000000 flopsy-0.0.2/flopsy/action.py
+drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-29 14:31:11.929724 flopsy-0.0.2/flopsy/inspector/
+-rw-r--r--   0 grib      (1000) grib      (1000)    10605 2023-04-23 20:26:12.000000 flopsy-0.0.2/flopsy/inspector/inspector.py
+-rw-r--r--   0 grib      (1000) grib      (1000)     2011 2023-04-22 20:00:32.000000 flopsy-0.0.2/flopsy/reducer.py
+-rw-r--r--   0 grib      (1000) grib      (1000)     1887 2023-04-29 14:09:08.000000 flopsy-0.0.2/flopsy/saga.py
+-rw-r--r--   0 grib      (1000) grib      (1000)     7965 2023-04-29 14:23:10.000000 flopsy-0.0.2/flopsy/store.py
+drwxr-xr-x   0 grib      (1000) grib      (1000)        0 2023-04-29 14:31:11.929724 flopsy-0.0.2/flopsy.egg-info/
+-rw-r--r--   0 grib      (1000) grib      (1000)      562 2023-04-29 14:31:11.000000 flopsy-0.0.2/flopsy.egg-info/PKG-INFO
+-rw-r--r--   0 grib      (1000) grib      (1000)      304 2023-04-29 14:31:11.000000 flopsy-0.0.2/flopsy.egg-info/SOURCES.txt
+-rw-r--r--   0 grib      (1000) grib      (1000)        1 2023-04-29 14:31:11.000000 flopsy-0.0.2/flopsy.egg-info/dependency_links.txt
+-rw-r--r--   0 grib      (1000) grib      (1000)       26 2023-04-29 14:31:11.000000 flopsy-0.0.2/flopsy.egg-info/requires.txt
+-rw-r--r--   0 grib      (1000) grib      (1000)        7 2023-04-29 14:31:11.000000 flopsy-0.0.2/flopsy.egg-info/top_level.txt
+-rw-r--r--   0 grib      (1000) grib      (1000)       79 2023-04-29 14:31:11.929724 flopsy-0.0.2/setup.cfg
+-rw-r--r--   0 grib      (1000) grib      (1000)      795 2023-04-26 16:47:38.000000 flopsy-0.0.2/setup.py
```

### Comparing `flopsy-0.0.1/LICENSE.txt` & `flopsy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flopsy-0.0.1/PKG-INFO` & `flopsy-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: flopsy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Redux-inspired state management
 Home-page: https://github.com/bgribble/flopsy
-Download-URL: https://github.com/bgribble/flopsy/archive/refs/tags/0.0.1.tar.gz
+Download-URL: https://github.com/bgribble/flopsy/archive/refs/tags/0.0.2.tar.gz
 Author: Bill Gribble
 Author-email: grib@billgribble.com
 License: MIT
 Keywords: state-management,redux,saga
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `flopsy-0.0.1/README.md` & `flopsy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flopsy-0.0.1/flopsy/inspector/inspector.py` & `flopsy-0.0.2/flopsy/inspector/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,37 +25,45 @@
         self.store_item_selected_value = None
 
         self.sagas = {}
         self.timeline = []
 
         self.event_loop = asyncio.get_event_loop()
 
-        for store_type in Store.all_store_types():
-            self.sagas[store_type.__name__] = store_type.install_saga(
-                self.update_timeline,
-            )
-
         self.initial_store = Store.store()
         self.initial_store_ts = datetime.now()
         self.current_store = copy.copy(self.initial_store)
 
+        self.store_listen()
+
     async def update_timeline(self, store, action, state_diff):
         self.timeline.append([
             datetime.now(),
             action,
             state_diff
         ])
         if self.timeline_item_selected is None:
             store_items = self.current_store.setdefault(store.store_type, {})
             store_item_content = store_items.setdefault(store.id, {})
 
             for state_key, values in state_diff.items():
                 store_item_content[state_key] = values[1]
         yield None
 
+    def store_listen(self):
+        for store_type in Store.all_store_types():
+            self.sagas[store_type.__name__] = store_type.install_saga(
+                self.update_timeline,
+            )
+
+    def store_unlisten(self):
+        for store_type in Store.all_store_types():
+            store_type.uninstall_saga(self.sagas[store_type.__name__])
+            del self.sagas[store_type.__name__]
+
     def store_dispatch_change(self, store_type, store_id, attr, value):
         store = Store.find_store(store_type, store_id)
         action = Action(
             target=store,
             type_name=f"SET_{attr.upper()}",
             payload=dict(value=value)
         )
@@ -131,14 +139,15 @@
                     self.current_store = Store.store()
                     self.timeline_item_selected = None
 
                 # Quit
                 clicked, rest = imgui.menu_item("Quit", "Ctrl+Q")
                 if clicked:
                     keep_going = False
+                    self.store_unlisten()
                 imgui.end_menu()
 
             imgui.end_main_menu_bar()
 
         # one window that fills the workspace
         imgui.set_next_window_size(self.window_width, self.window_height-21)
         imgui.set_next_window_position(0, 21)
```

### Comparing `flopsy-0.0.1/flopsy/reducer.py` & `flopsy-0.0.2/flopsy/reducer.py`

 * *Files identical despite different names*

### Comparing `flopsy-0.0.1/flopsy/saga.py` & `flopsy-0.0.2/flopsy/saga.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,20 +39,18 @@
             return self.func(*args, **kwargs)
 
     def _assign_func(self, func):
         self.func = func
         self.action_name = func.__name__.upper()
         self.method_name = '_' + self.action_name
 
-    # __set_name__ gets called because @reducer is a "descriptor",
+    # __set_name__ gets called because @saga is a "descriptor",
     # at the right time in the init process
     def __set_name__(self, owner, name):
         self.owning_class = owner
         setattr(owner, self.method_name, self.func)
         setattr(owner, self.action_name, self.action_name)
 
-        if self.states is None:
-            self.states = self.owning_class.store_attrs
         saga_id = self.owning_class._next_saga_id
         self.owning_class._next_saga_id += 1
         self.owning_class._store_sagas.append((saga_id, self, self.states))
```

### Comparing `flopsy-0.0.1/flopsy/store.py` & `flopsy-0.0.2/flopsy/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
 import asyncio
+import logging
+
 from .action import Action
 
 
 class Store:
     """
     Base class for stores of managed state
 
@@ -24,30 +26,35 @@
     id for the store, to be used when aggregating the
     application's stores. Defaults to "id"
     """
     _store_registry = {}
     _store_reducers = {}
     _store_sagas = []
     _store_tasks = []
+    _store_logger = None
 
     _next_saga_id = 1
     _next_reducer_id = 1
+    _next_default_id = 1
 
     @classmethod
     def _setter_helper(cls, attr):
         def inner(self, newval):
             oldval = getattr(self, attr)
             setattr(self, attr, newval)
             return (attr, oldval)
         return inner
 
     def __init_subclass__(cls):
         if not hasattr(cls, 'store_attrs'):
             return
 
+        if not hasattr(cls, 'store_type'):
+            cls.store_type = cls.__name__
+
         Store._store_registry[cls.__name__] = {}
 
         for attr in cls.store_attrs:
             setter_action = f"SET_{attr.upper()}"
             setter_methodname = f"_{setter_action}"
             setter_dispatch = cls._setter_helper(attr)
 
@@ -58,16 +65,24 @@
             setattr(cls, getter_statename, attr)
 
             # define the setter as a method
             setattr(cls, setter_methodname, setter_dispatch)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        id_attr = getattr(self, "store_id_attr", "id")
-        Store._store_registry[type(self).__name__][getattr(self, id_attr)] = self
+        id_attr = getattr(self, "store_id_attr", None)
+        if id_attr is None:
+            id_attr = "id"
+            id_value = Store._next_default_id
+            Store._next_default_id += 1
+            setattr(self, id_attr, id_value)
+
+        Store._store_registry[
+            type(self).__name__
+        ][getattr(self, id_attr)] = self
 
     def action(self, action_label, **kwargs):
         return Action(self, action_label, kwargs)
 
     def state(self, label=None):
         if not label:
             return {
@@ -92,16 +107,14 @@
                 magic_handler = getattr(self, magic_handler_name)
                 new_value = action.payload.get("value", None)
                 state_name, old_value = magic_handler(new_value)
                 if old_value != new_value:
                     state_diff[state_name] = (old_value, new_value)
 
         changed_state_set = set(state_diff.keys())
-        if not changed_state_set:
-            return
 
         for callback_id, callback, state_filter in self._store_sagas:
             if state_filter and not (set(state_filter) & changed_state_set):
                 continue
             self._launch_task(
                 self._run_saga(
                     callback(self, action, state_diff)
@@ -115,17 +128,20 @@
             if t and not t.done()
         ]
 
         # save the new one
         Store._store_tasks.append(asyncio.create_task(task))
 
     async def _run_saga(self, saga):
-        async for action in saga:
-            if action and isinstance(action, Action):
-                await self.dispatch(action)
+        try:
+            async for action in saga:
+                if action and isinstance(action, Action):
+                    await self.dispatch(action)
+        except Exception as e:
+            Store.log(f"Exception in saga {saga}: {e}")
 
     # install reducer for states
     @classmethod
     def install_reducer(cls, action_name, states):
 
         reducer_id = Store._next_reducer_id
         Store._next_reducer_id += 1
@@ -194,14 +210,21 @@
     @staticmethod
     def show_inspector():
         from .inspector.inspector import Inspector
         inspector = Inspector()
         inspector.start()
         return inspector
 
+    @staticmethod
+    def log(*args):
+        if not Store._store_logger:
+            Store._store_logger = logging.getLogger(__name__)
+        Store._store_logger.error(*args)
+
+
 class SyncedStore (Store):
     """
     A type of store with convenience actions for syncing
     with a remote source of truth.
 
     In addition to the normal setters, attr "my_attr" will
     also have a secondary setter action called
```

### Comparing `flopsy-0.0.1/flopsy.egg-info/PKG-INFO` & `flopsy-0.0.2/flopsy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: flopsy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Redux-inspired state management
 Home-page: https://github.com/bgribble/flopsy
-Download-URL: https://github.com/bgribble/flopsy/archive/refs/tags/0.0.1.tar.gz
+Download-URL: https://github.com/bgribble/flopsy/archive/refs/tags/0.0.2.tar.gz
 Author: Bill Gribble
 Author-email: grib@billgribble.com
 License: MIT
 Keywords: state-management,redux,saga
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `flopsy-0.0.1/setup.py` & `flopsy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 
 # build with 'python ./setup.py install'
 from distutils.core import setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 setup(
     name = 'flopsy',
     version = VERSION,
     license = 'MIT',
     description = 'Redux-inspired state management',
     author = 'Bill Gribble',
     author_email = 'grib@billgribble.com',
     url = 'https://github.com/bgribble/flopsy',
-    download_url = 'https://github.com/bgribble/flopsy/archive/refs/tags/0.0.1.tar.gz',
+    download_url = 'https://github.com/bgribble/flopsy/archive/refs/tags/0.0.2.tar.gz',
     keywords = ['state-management', 'redux', 'saga'],
     install_requires = [
         'pyopengl', 'glfw', 'imgui[glfw]',
     ],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```


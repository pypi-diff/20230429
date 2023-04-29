# Comparing `tmp/reactives-0.4.3.tar.gz` & `tmp/reactives-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactives-0.4.3.tar", last modified: Wed Dec  7 20:18:30 2022, max compression
+gzip compressed data, was "reactives-0.5.0.tar", last modified: Sat Apr 29 09:37:29 2023, max compression
```

## Comparing `reactives-0.4.3.tar` & `reactives-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.202580 reactives-0.4.3/
--rw-rw-r--   0 bart      (1000) bart      (1000)    32453 2021-05-15 15:57:10.000000 reactives-0.4.3/LICENSE.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)    10719 2022-12-07 20:18:30.202580 reactives-0.4.3/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)     9928 2022-12-07 20:18:13.000000 reactives-0.4.3/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2022-12-07 20:18:29.000000 reactives-0.4.3/VERSION
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.198580 reactives-0.4.3/reactives/
--rw-rw-r--   0 bart      (1000) bart      (1000)      296 2022-03-25 18:25:03.000000 reactives-0.4.3/reactives/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7597 2022-03-25 18:25:03.000000 reactives-0.4.3/reactives/collections.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.198580 reactives-0.4.3/reactives/factory/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1916 2022-03-25 18:25:03.000000 reactives-0.4.3/reactives/factory/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3320 2022-04-05 19:11:05.000000 reactives-0.4.3/reactives/factory/function.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4736 2022-05-03 18:36:23.000000 reactives-0.4.3/reactives/factory/property.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5794 2022-04-05 19:11:05.000000 reactives-0.4.3/reactives/factory/type.py
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-03-17 23:28:35.000000 reactives-0.4.3/reactives/py.typed
--rw-rw-r--   0 bart      (1000) bart      (1000)     9404 2022-12-07 20:18:13.000000 reactives-0.4.3/reactives/reactor.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1746 2022-05-03 16:31:15.000000 reactives-0.4.3/reactives/scope.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.202580 reactives-0.4.3/reactives/tests/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2760 2022-12-07 20:18:13.000000 reactives-0.4.3/reactives/tests/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.202580 reactives-0.4.3/reactives/tests/factory/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-03-17 23:28:35.000000 reactives-0.4.3/reactives/tests/factory/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      256 2022-03-25 18:25:03.000000 reactives-0.4.3/reactives/tests/factory/test___init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4363 2022-04-05 19:11:05.000000 reactives-0.4.3/reactives/tests/factory/test_function.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8910 2022-05-03 18:36:23.000000 reactives-0.4.3/reactives/tests/factory/test_property.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5220 2022-04-05 19:11:05.000000 reactives-0.4.3/reactives/tests/factory/test_type.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    23326 2022-03-17 23:28:35.000000 reactives-0.4.3/reactives/tests/test_collections.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6480 2022-12-07 20:18:13.000000 reactives-0.4.3/reactives/tests/test_reactor.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      807 2022-03-25 18:25:03.000000 reactives-0.4.3/reactives/tests/test_scope.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-07 20:18:30.198580 reactives-0.4.3/reactives.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)    10719 2022-12-07 20:18:29.000000 reactives-0.4.3/reactives.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)      746 2022-12-07 20:18:30.000000 reactives-0.4.3/reactives.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2022-12-07 20:18:29.000000 reactives-0.4.3/reactives.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      294 2022-12-07 20:18:30.000000 reactives-0.4.3/reactives.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       10 2022-12-07 20:18:30.000000 reactives-0.4.3/reactives.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2022-12-07 20:18:30.202580 reactives-0.4.3/setup.cfg
--rw-rw-r--   0 bart      (1000) bart      (1000)     2219 2022-12-07 14:29:41.000000 reactives-0.4.3/setup.py
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:29.320839 reactives-0.5.0/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)    32453 2023-04-29 08:44:23.000000 reactives-0.5.0/LICENSE.txt
+-rwxrwxrwx   0 bart      (1000) bart      (1000)    10273 2023-04-29 09:37:29.315965 reactives-0.5.0/PKG-INFO
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     9453 2023-04-29 08:44:23.000000 reactives-0.5.0/README.md
+-rwxrwxrwx   0 bart      (1000) bart      (1000)        6 2023-04-29 09:37:08.000000 reactives-0.5.0/VERSION
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:28.420842 reactives-0.5.0/reactives/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)      431 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/__init__.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     1778 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/_callable.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)      204 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/_decorator.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     9736 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/collections.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     2050 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/function.py
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:28.766676 reactives-0.5.0/reactives/instance/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     9235 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/instance/__init__.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     4082 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/instance/method.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     4715 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/instance/property.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/py.typed
+-rwxrwxrwx   0 bart      (1000) bart      (1000)    11903 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/reactor.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     2164 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/scope.py
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:29.035326 reactives-0.5.0/reactives/tests/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     2400 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/__init__.py
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:29.263857 reactives-0.5.0/reactives/tests/instance/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/instance/__init__.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     5638 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/instance/test___init__.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     4187 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/instance/test_method.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     7817 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/instance/test_property.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     1467 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/test__callable.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)    23423 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/test_collections.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     2238 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/test_function.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     9712 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/test_reactor.py
+-rwxrwxrwx   0 bart      (1000) bart      (1000)      795 2023-04-29 08:44:23.000000 reactives-0.5.0/reactives/tests/test_scope.py
+drwxrwxrwx   0 bart      (1000) bart      (1000)        0 2023-04-29 09:37:28.606866 reactives-0.5.0/reactives.egg-info/
+-rwxrwxrwx   0 bart      (1000) bart      (1000)    10273 2023-04-29 09:37:23.000000 reactives-0.5.0/reactives.egg-info/PKG-INFO
+-rwxrwxrwx   0 bart      (1000) bart      (1000)      822 2023-04-29 09:37:25.000000 reactives-0.5.0/reactives.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bart      (1000) bart      (1000)        1 2023-04-29 09:37:23.000000 reactives-0.5.0/reactives.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bart      (1000) bart      (1000)      303 2023-04-29 09:37:23.000000 reactives-0.5.0/reactives.egg-info/requires.txt
+-rwxrwxrwx   0 bart      (1000) bart      (1000)       10 2023-04-29 09:37:23.000000 reactives-0.5.0/reactives.egg-info/top_level.txt
+-rwxrwxrwx   0 bart      (1000) bart      (1000)       38 2023-04-29 09:37:29.322842 reactives-0.5.0/setup.cfg
+-rwxrwxrwx   0 bart      (1000) bart      (1000)     2280 2023-04-29 09:36:05.000000 reactives-0.5.0/setup.py
```

### Comparing `reactives-0.4.3/LICENSE.txt` & `reactives-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `reactives-0.4.3/PKG-INFO` & `reactives-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: reactives
-Version: 0.4.3
+Version: 0.5.0
 Summary: A declarative reactive programming framework.
 Home-page: https://github.com/bartfeenstra/reactives
 Author: Bart Feenstra & contributors
 Author-email: bart@mynameisbart.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~= 3.7
+Classifier: Typing :: Typed
+Requires-Python: ~= 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: development
 License-File: LICENSE.txt
 
 
 # Reactives
 
@@ -30,166 +31,140 @@
 its reactors and its reactors' reactors are resolved, and each is called once in order.
 
 **Reactives** uses a push-pull approach, meaning change notifications are pushed (reactors are called automatically and
 won't have to pull for changes), but if a reactor needs to know what exactly changed, it must pull this information
 itself.
 
 ## Usage
-For any type to be reactive, it must extend `reactives.factory.Reactive` and set a `reactives.ReactorController`
-instance in its `__init__()` method. For any of the types supported by default, you only have to decorate your type or
-value with `@reactives.reactive`. Additionally, some classes are provided that are reactive and can be instantiated or
-inherited from directly.
+For any type to be reactive, it must extend `reactives.Reactive` and expose a `reactives.reactor.ReactorController`
+instance through its `react` instance attribute.
+
+**Reactives** provides the reactive framework, the tools to make your own types reactive, and several fully reactive
+types out of the box, batteries included!
 
 ### Custom classes
 Decorate a class to make its individual instances reactive:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     pass
 
 apple = Apple()
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 ### Functions and methods 
 Decorate a function:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive
+@reactive_function
 def apple():
     pass
 
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 Decorate a method on a **reactive class**:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.method import reactive_method
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
+    @reactive_method
     def apple(self):
         pass
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 Reactive methods must be accessed through their instance, because `Apple.apple` would yield the class method.
 
 Both functions and methods can be called automatically when they're triggered. This lets them set up something once, and
 update that thing when they're triggered:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive(on_trigger_call=True)
+@reactive_function(on_trigger_call=True)
 def warm_caches():
     """
     Warm the application's caches. When triggered (because the cached data has changed), re-warm the caches.
     """
     pass
 ```
 
 ### Properties
 Decorate a property:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
     @property
+    @reactive_property
     def apple(self) -> str:
         return 'I got you something!'
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 
-If a property *deleter* is present, it will be called automatically when the property is triggered:
+If a property *deleter* is present, it may be called automatically when the property is triggered:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._cached_something = None
 
-    @reactive
     @property
+    @reactive_property(on_trigger_delete=True)
     def apple(self) -> str:
         if self._cached_something is None:
             self._cached_something = 'I got you something!'
         return self._cached_something
 
     @apple.deleter
     def apple(self)  -> None:
         self._cached_something = 'I got you nothing!'
 
 apple = Apple()
 print(apple.apple)
 # >>> "I got you something!"
-apple.react['apple'].react().trigger()
+apple.react['apple'].react.trigger()
 print(apple.apple)
 # >>> "I got you nothing!"
 ```
 
-If you do not want automatic deletion, configure the property's `@reactive` decorator as such:
-```python
-from reactives import reactive
-
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(on_trigger_delete=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            self._cached_something = 'I got you something!'
-        return self._cached_something
-
-    @apple.deleter
-    def apple(self)  -> None:
-        self._cached_something = 'I got you nothing!'
-
-apple = Apple()
-print(apple.apple)
-# >>> "I got you something!"
-apple.react['apple'].react().trigger()
-print(apple.apple)
-# >>> "I got you something!"
-```
-
 Property *setters* work exactly like with any other `property`:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._something = 'I got you something!'
-        
-    @reactive
+
     @property
+    @reactive_property
     def apple(self) -> str:
         return self._something
-    
+
     @apple.setter
     def apple(self, something: str):
         self._something = something
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.apple = 'I got you something else!'
@@ -197,71 +172,51 @@
 ```
 
 Values set through a property may themselves be reactive too. If they are, the property and the value are autowired, 
 which means that the property becomes a reactor to the newly added value. As soon as the value is triggered,
 so is the property. Therefore, if you want to react to any change to any of the values a property might have, all you
 need to do is add your reactor to the property.
 
-*Getters* that perform conditional logic, such as for cached properties, can take over reactive scope dependency
-collection for more fine-grained reactivity control:
-```python
-from reactives import reactive, scope
-
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(auto_collect_scope=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            with scope.collect(self.react['apple']):
-                self._cached_something = build_something()
-        return self._cached_something
-
-def build_something():
-    pass
-```
-
-### Lists
-`ReactiveList` is a reactive version of Python's built-in `list`. You can use it in exactly the same way as `list`:
+### Sequences
+`reactives.collections.ReactiveSequence` and `reactives.collections.ReactiveMutableSequence` are reactive versions of 
+Python's built-in `Sequence` and `MutableSequence`, which are drop-in replacements for `list`.
 ```python
-from reactives import ReactiveList
+from reactives.collections import ReactiveMutableSequence
 
-fruits = ReactiveList(['apple', 'banana'])
+fruits = ReactiveMutableSequence(['apple', 'banana'])
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits.append('orange')
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveList` may themselves be reactive too. If they are, the list and the value are autowired, 
-which means that the list becomes a reactor to the newly added value. As soon as the value is triggered,
-so is the list. Therefore, if you want to react to any change to any of the values in a `ReactiveList`, all you
-need to do is add your reactor to the list.
-
-### Dictionaries
-`ReactiveDict` is a reactive version of Python's built-in `dict`. You can use it in exactly the same way as `dict`:
+Values added to a `ReactiveSequence` or `ReactiveMutableSequence` may themselves be reactive too. If they are, the 
+sequence and the value are autowired, which means that the sequence becomes a reactor to the newly added value. As soon 
+as the value is triggered, so is the sequence. Therefore, if you want to react to any change to any of the values in a
+`ReactiveSequence` or `ReactiveMutableSequence`, all you need to do is add your reactor to the sequence.
+
+### Mappings
+`reactives.collections.ReactiveMapping` and `reactives.collections.ReactiveMutableMapping` are reactive versions of 
+Python's built-in `Mapping` and `MutableMapping`, which are drop-in replacements for `dict`.
 ```python
-from reactives import ReactiveDict
+from reactives.collections import ReactiveMutableMapping
 
-fruits = ReactiveDict(apple=5, banana=2)
+fruits = ReactiveMutableMapping(apple=5, banana=2)
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits['orange'] = 4
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveDict` may themselves be reactive too. If they are, the dictionary and the value are
-autowired, which means that the dictionary becomes a reactor to the newly added value. As soon as the value is
-triggered, so is the dictionary. Therefore, if you want to react to any change to any of the values in a `ReactiveDict`, 
-all you  need to do is add your reactor to the dictionary.
+Values added to a `ReactiveMapping` or `ReactiveMutableMapping` may themselves be reactive too. If they are, the 
+mapping and the value are autowired, which means that the mapping becomes a reactor to the newly added value. As soon as
+the value is triggered, so is the mapping. Therefore, if you want to react to any change to any of the values in a 
+`ReactiveMapping` or `ReactiveMutableMapping`, all you  need to do is add your reactor to the mapping.
 
 ### Autowiring
-We've seen how [properties](#Properties), [lists](#Lists), and [dictionaries](#Dictionaries) autowire themselves to
-their values. This is possible because properties, lists, and dictionaries know exactly which values move in and out of
+We've seen how [properties](#Properties), [sequences](#Sequences), and [mappings](#Mappings) autowire themselves to
+their values. This is possible because properties, sequences, and mappings know exactly which values move in and out of
 them. In other cases, we use *scope*. Any reactive can start a scope with `reactives.scope.collect()` and collect all
 reactives that are called or used during that scope window, and autowire itself to them. Conversely, any reactive can
 register itself with the current scope (if there is one) with `reactives.scope.register*()`, and allow reactives
 depending on it to autowire themselves. In fact, this is what properties do internally.
 
 Autowiring means that as a developer, you won't need to worry about connecting the parts of your application most of the
 time.
```

### Comparing `reactives-0.4.3/README.md` & `reactives-0.5.0/reactives.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: reactives
+Version: 0.5.0
+Summary: A declarative reactive programming framework.
+Home-page: https://github.com/bartfeenstra/reactives
+Author: Bart Feenstra & contributors
+Author-email: bart@mynameisbart.com
+License: GPLv3
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Typing :: Typed
+Requires-Python: ~= 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: development
+License-File: LICENSE.txt
+
 
 # Reactives
 
 ![Test status](https://github.com/bartfeenstra/reactives/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/reactives/branch/main/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/reactives) [![PyPI releases](https://badge.fury.io/py/reactives.svg)](https://pypi.org/project/reactives/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/reactives.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/reactives/) [![Recent downloads](https://img.shields.io/pypi/dm/reactives.svg)](https://pypi.org/project/reactives/) 
 
 **Reactives** lets you write reactive code easily by making any of your objects and functions *reactive*. A reactive
 can be *triggered* (`reactive.react.trigger()`), causing all its *reactors* to be called. A *reactor* is any callable
@@ -9,166 +31,140 @@
 its reactors and its reactors' reactors are resolved, and each is called once in order.
 
 **Reactives** uses a push-pull approach, meaning change notifications are pushed (reactors are called automatically and
 won't have to pull for changes), but if a reactor needs to know what exactly changed, it must pull this information
 itself.
 
 ## Usage
-For any type to be reactive, it must extend `reactives.factory.Reactive` and set a `reactives.ReactorController`
-instance in its `__init__()` method. For any of the types supported by default, you only have to decorate your type or
-value with `@reactives.reactive`. Additionally, some classes are provided that are reactive and can be instantiated or
-inherited from directly.
+For any type to be reactive, it must extend `reactives.Reactive` and expose a `reactives.reactor.ReactorController`
+instance through its `react` instance attribute.
+
+**Reactives** provides the reactive framework, the tools to make your own types reactive, and several fully reactive
+types out of the box, batteries included!
 
 ### Custom classes
 Decorate a class to make its individual instances reactive:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     pass
 
 apple = Apple()
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 ### Functions and methods 
 Decorate a function:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive
+@reactive_function
 def apple():
     pass
 
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 Decorate a method on a **reactive class**:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.method import reactive_method
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
+    @reactive_method
     def apple(self):
         pass
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 Reactive methods must be accessed through their instance, because `Apple.apple` would yield the class method.
 
 Both functions and methods can be called automatically when they're triggered. This lets them set up something once, and
 update that thing when they're triggered:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive(on_trigger_call=True)
+@reactive_function(on_trigger_call=True)
 def warm_caches():
     """
     Warm the application's caches. When triggered (because the cached data has changed), re-warm the caches.
     """
     pass
 ```
 
 ### Properties
 Decorate a property:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
     @property
+    @reactive_property
     def apple(self) -> str:
         return 'I got you something!'
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 
-If a property *deleter* is present, it will be called automatically when the property is triggered:
+If a property *deleter* is present, it may be called automatically when the property is triggered:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._cached_something = None
 
-    @reactive
     @property
+    @reactive_property(on_trigger_delete=True)
     def apple(self) -> str:
         if self._cached_something is None:
             self._cached_something = 'I got you something!'
         return self._cached_something
 
     @apple.deleter
     def apple(self)  -> None:
         self._cached_something = 'I got you nothing!'
 
 apple = Apple()
 print(apple.apple)
 # >>> "I got you something!"
-apple.react['apple'].react().trigger()
+apple.react['apple'].react.trigger()
 print(apple.apple)
 # >>> "I got you nothing!"
 ```
 
-If you do not want automatic deletion, configure the property's `@reactive` decorator as such:
-```python
-from reactives import reactive
-
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(on_trigger_delete=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            self._cached_something = 'I got you something!'
-        return self._cached_something
-
-    @apple.deleter
-    def apple(self)  -> None:
-        self._cached_something = 'I got you nothing!'
-
-apple = Apple()
-print(apple.apple)
-# >>> "I got you something!"
-apple.react['apple'].react().trigger()
-print(apple.apple)
-# >>> "I got you something!"
-```
-
 Property *setters* work exactly like with any other `property`:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._something = 'I got you something!'
-        
-    @reactive
+
     @property
+    @reactive_property
     def apple(self) -> str:
         return self._something
-    
+
     @apple.setter
     def apple(self, something: str):
         self._something = something
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.apple = 'I got you something else!'
@@ -176,71 +172,51 @@
 ```
 
 Values set through a property may themselves be reactive too. If they are, the property and the value are autowired, 
 which means that the property becomes a reactor to the newly added value. As soon as the value is triggered,
 so is the property. Therefore, if you want to react to any change to any of the values a property might have, all you
 need to do is add your reactor to the property.
 
-*Getters* that perform conditional logic, such as for cached properties, can take over reactive scope dependency
-collection for more fine-grained reactivity control:
+### Sequences
+`reactives.collections.ReactiveSequence` and `reactives.collections.ReactiveMutableSequence` are reactive versions of 
+Python's built-in `Sequence` and `MutableSequence`, which are drop-in replacements for `list`.
 ```python
-from reactives import reactive, scope
+from reactives.collections import ReactiveMutableSequence
 
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(auto_collect_scope=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            with scope.collect(self.react['apple']):
-                self._cached_something = build_something()
-        return self._cached_something
-
-def build_something():
-    pass
-```
-
-### Lists
-`ReactiveList` is a reactive version of Python's built-in `list`. You can use it in exactly the same way as `list`:
-```python
-from reactives import ReactiveList
-
-fruits = ReactiveList(['apple', 'banana'])
+fruits = ReactiveMutableSequence(['apple', 'banana'])
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits.append('orange')
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveList` may themselves be reactive too. If they are, the list and the value are autowired, 
-which means that the list becomes a reactor to the newly added value. As soon as the value is triggered,
-so is the list. Therefore, if you want to react to any change to any of the values in a `ReactiveList`, all you
-need to do is add your reactor to the list.
-
-### Dictionaries
-`ReactiveDict` is a reactive version of Python's built-in `dict`. You can use it in exactly the same way as `dict`:
+Values added to a `ReactiveSequence` or `ReactiveMutableSequence` may themselves be reactive too. If they are, the 
+sequence and the value are autowired, which means that the sequence becomes a reactor to the newly added value. As soon 
+as the value is triggered, so is the sequence. Therefore, if you want to react to any change to any of the values in a
+`ReactiveSequence` or `ReactiveMutableSequence`, all you need to do is add your reactor to the sequence.
+
+### Mappings
+`reactives.collections.ReactiveMapping` and `reactives.collections.ReactiveMutableMapping` are reactive versions of 
+Python's built-in `Mapping` and `MutableMapping`, which are drop-in replacements for `dict`.
 ```python
-from reactives import ReactiveDict
+from reactives.collections import ReactiveMutableMapping
 
-fruits = ReactiveDict(apple=5, banana=2)
+fruits = ReactiveMutableMapping(apple=5, banana=2)
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits['orange'] = 4
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveDict` may themselves be reactive too. If they are, the dictionary and the value are
-autowired, which means that the dictionary becomes a reactor to the newly added value. As soon as the value is
-triggered, so is the dictionary. Therefore, if you want to react to any change to any of the values in a `ReactiveDict`, 
-all you  need to do is add your reactor to the dictionary.
+Values added to a `ReactiveMapping` or `ReactiveMutableMapping` may themselves be reactive too. If they are, the 
+mapping and the value are autowired, which means that the mapping becomes a reactor to the newly added value. As soon as
+the value is triggered, so is the mapping. Therefore, if you want to react to any change to any of the values in a 
+`ReactiveMapping` or `ReactiveMutableMapping`, all you  need to do is add your reactor to the mapping.
 
 ### Autowiring
-We've seen how [properties](#Properties), [lists](#Lists), and [dictionaries](#Dictionaries) autowire themselves to
-their values. This is possible because properties, lists, and dictionaries know exactly which values move in and out of
+We've seen how [properties](#Properties), [sequences](#Sequences), and [mappings](#Mappings) autowire themselves to
+their values. This is possible because properties, sequences, and mappings know exactly which values move in and out of
 them. In other cases, we use *scope*. Any reactive can start a scope with `reactives.scope.collect()` and collect all
 reactives that are called or used during that scope window, and autowire itself to them. Conversely, any reactive can
 register itself with the current scope (if there is one) with `reactives.scope.register*()`, and allow reactives
 depending on it to autowire themselves. In fact, this is what properties do internally.
 
 Autowiring means that as a developer, you won't need to worry about connecting the parts of your application most of the
 time.
@@ -269,7 +245,9 @@
 [submit improvements](https://github.com/bartfeenstra/reactives/pulls).
 
 ## Copyright & license
 Reactives is copyright [Bart Feenstra](https://twitter.com/BartFeenstra/) and contributors, and released under the
 [GNU General Public License, Version 3](./LICENSE.txt). In short, that means **you are free to use Reactives**, but **if you
 distribute Reactives yourself, you must do so under the exact same license**, provide that license, and make your source
 code available. 
+
+
```

### Comparing `reactives-0.4.3/reactives/factory/type.py` & `reactives-0.5.0/reactives/tests/instance/test___init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,157 @@
+from __future__ import annotations
+
 import copy
-import functools
-import inspect
-from contextlib import suppress
-from typing import Dict, Any, Type
-from warnings import warn
+import pickle
+
+import pytest
+
+from reactives import Reactive
+from reactives.instance import ReactiveInstance, _ReactiveInstanceReactorController, InstanceAttributeDefinition
+from reactives.instance.method import reactive_method
+from reactives.tests import assert_reactor_called, assert_not_reactor_called
 
 try:
-    from typing import Self  # type: ignore
+    from typing_extensions import Self
 except ImportError:
-    from typing_extensions import Self  # type: ignore
+    from typing import Self  # type: ignore
 
-from reactives.factory import reactive_factory, Reactive
-from reactives.reactor import ReactorController
 
+class Subject(ReactiveInstance):
+    @reactive_method
+    def subject_method(self) -> None:
+        pass
+
+    @property
+    @reactive_method
+    def subject_property(self) -> None:
+        return
 
-class InstanceAttribute:
-    def create_instance_attribute_reactor_controller(self, instance) -> ReactorController:
-        raise NotImplementedError
-
-
-class _ReactiveInstanceAttribute(Reactive):
-    def __init__(self, reactor_controller: ReactorController):
-        self.react = reactor_controller
-
-
-class _InstanceReactorController(ReactorController):
-    def __init__(self, instance):
-        super().__init__()
-        self._instance = instance
-        self._reactive_attributes: Dict[Any, _ReactiveInstanceAttribute] = {}
-        self._initialized = False
-
-    def copy_for_instance(self, instance: Any):
-        copied = copy.copy(self)
-        copied._instance = instance
-        self._rewire_to_copy(copied)
-        return copied
-
-    def _rewire_to_copy(self, copied: '_InstanceReactorController') -> None:
-        for reactive_attr_name, reactive_attribute in copied._reactive_attributes.items():
-            with suppress(ValueError):
-                copied._reactive_attributes[reactive_attr_name].react.shutdown(self._instance)
-            copied._reactive_attributes[reactive_attr_name].react(copied._instance)
-
-    def __getstate__(self) -> Dict[str, Any]:
-        state = super().__getstate__()
-        state['_instance'] = self._instance
-        state['_reactive_attributes'] = {
-            reactive_attr_name: reactive_attribute
-            for reactive_attr_name, reactive_attribute in self._reactive_attributes.items()
-            # Filter out reactive attributes set by value, and keep those set by attribute name. The value keys will be
-            # restored upon unpickling.
-            if isinstance(reactive_attr_name, str)
-        }
-        return state
-
-    def __setstate__(self, state: Dict[str, Any]) -> None:
-        super().__setstate__(state)
-        self._instance = state['_instance']
-        self._reactive_attributes = {}
-        self._reactive_attributes = state['_reactive_attributes']
-        self._initialized = False
 
+class SubjectWithCopy(Subject):
     def __copy__(self) -> Self:
-        self._initialize_reactive_instance_attributes()
-        copied = super().__copy__()
-        copied._instance = self._instance
-        copied._reactive_attributes = copy.copy(self._reactive_attributes)
-        copied._initialized = True
-        return copied
-
-    def _initialize_reactive_instance_attributes(self) -> None:
-        if self._initialized:
-            return
-        self._initialized = True
-
-        for reactive_attr_name, reactive_attr_value in inspect.getmembers(self._instance.__class__, lambda x: isinstance(x, InstanceAttribute)):
-            self._initialize_reactive_attribute(reactive_attr_name, reactive_attr_value)
-
-    def _initialize_reactive_attribute(self, reactive_attr_name: str, reactive_attr_value: Any) -> None:
-        if reactive_attr_name in self._reactive_attributes:
-            # When pickling or copying, reactive attributes with non-string keys are omitted. We must recover those
-            # here.
-            self._reactive_attributes[reactive_attr_value] = self._reactive_attributes[reactive_attr_name]
-            return
-
-        reactor_controller = reactive_attr_value.create_instance_attribute_reactor_controller(self._instance)
-        reactive_attribute = _ReactiveInstanceAttribute(reactor_controller)
-        reactive_attribute.react(self._instance)
-        # Store reactive attributes by name as well as their original value, as we need access through both.
-        self._reactive_attributes[reactive_attr_name] = self._reactive_attributes[reactive_attr_value] = reactive_attribute
-
-    def getattr(self, name_or_attribute: Any) -> Reactive:
-        """
-        Get a reactive instance attribute.
-        """
-        self._initialize_reactive_instance_attributes()
-        try:
-            return self._reactive_attributes[name_or_attribute]
-        except KeyError:
-            raise AttributeError(f'No reactive attribute "{name_or_attribute}" exists.')
-
-    def __getitem__(self, name_or_attribute: Any) -> Reactive:
-        return self.getattr(name_or_attribute)
-
-
-class ReactiveInstance(Reactive):
-    """
-    Define a reactive instance.
-
-    Although this does not extend reactives.factory.Reactive, it will pass isinstance(x, reactives.factory.Reactive)
-    checks.
-    """
-
-    react: _InstanceReactorController
-
-
-@reactive_factory(type)
-def _reactive_type(decorated_class: Type[ReactiveInstance]) -> Type[ReactiveInstance]:
-    if not issubclass(decorated_class, ReactiveInstance):
-        warn(f'{decorated_class} was made reactive. For accurate type hinting it must also extend `{ReactiveInstance}`.', stacklevel=2)
-
-    # Override the initializer to instantiate an instance-level reactor controller.
-    original_init = decorated_class.__init__
-
-    @functools.wraps(original_init)
-    def _init(self, *args, **kwargs):
-        self.react = _InstanceReactorController(self)
-        original_init(self, *args, **kwargs)
-    setattr(decorated_class, '__init__', _init)
-
-    original_copy = getattr(decorated_class, '__copy__', None)
-
-    def _copy(self):
-        if original_copy is not None:
-            copied = original_copy(self)
-        else:
-            copied = self.__class__.__new__(self.__class__)
-
-        copied.react = self.react.copy_for_instance(copied)
-
-        return copied
-    if original_copy is not None:
-        functools.update_wrapper(_copy, original_copy)
-    setattr(decorated_class, '__copy__', _copy)
+        return self.__class__()
+
 
-    return decorated_class
+class SubjectWithNonReactiveAttribute(ReactiveInstance):
+    def subject(self) -> None:
+        pass
+
+
+class SubjectWithoutAttributes(ReactiveInstance):
+    pass
+
+
+class TestReactiveInstanceReactorController:
+    def test___copy__(self) -> None:
+        sut = _ReactiveInstanceReactorController(Subject())
+        with assert_reactor_called(sut):
+            copied_sut = copy.copy(sut)
+            with assert_not_reactor_called(sut):
+                with assert_reactor_called(copied_sut):
+                    copied_sut.trigger()
+
+    def test_getattr_with_reactive_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(Subject())
+        assert isinstance(sut.getattr_reactive('subject_method'), Reactive)
+
+    def test_getattr_with_existent_non_reactive_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(SubjectWithNonReactiveAttribute())
+        with pytest.raises(AttributeError):
+            sut.getattr_reactive('subject_method')
+
+    def test_getattr_with_non_existent_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(SubjectWithoutAttributes())
+        with pytest.raises(AttributeError):
+            sut.getattr_reactive('subject_method')
+
+    def test___getitem___with_reactive_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(Subject())
+        assert isinstance(sut['subject_method'], Reactive)
+
+    def test___getitem___with_existent_non_reactive_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(SubjectWithoutAttributes())
+        with pytest.raises(AttributeError):
+            sut['subject']
+
+    def test___getitem___with_non_existent_attribute(self) -> None:
+        sut = _ReactiveInstanceReactorController(SubjectWithoutAttributes())
+        with pytest.raises(AttributeError):
+            sut['subject']
+
+
+class TestReactiveInstance:
+    def test_pickle(self) -> None:
+        subject = Subject()
+        unpickled_subject = pickle.loads(pickle.dumps(subject))
+        with assert_not_reactor_called(subject):
+            with assert_reactor_called(unpickled_subject):
+                unpickled_subject.react.trigger()
+
+    def test___copy___without___copy__(self) -> None:
+        subject = Subject()
+        copied_subject = copy.copy(subject)
+        with assert_not_reactor_called(subject):
+            with assert_reactor_called(copied_subject):
+                copied_subject.react.trigger()
+
+    def test___copy___with___copy__(self) -> None:
+        subject = SubjectWithCopy()
+        copied_subject = copy.copy(subject)
+        with assert_not_reactor_called(subject):
+            with assert_reactor_called(copied_subject):
+                copied_subject.react.trigger()
+
+    def test_instance_trigger_without_reactors(self) -> None:
+        Subject().react.trigger()
+
+    def test_instance_trigger_with_instance_reactor(self) -> None:
+        subject = Subject()
+        with assert_reactor_called(subject):
+            subject.react.trigger()
+
+    def test_instance_trigger_with_instance_attribute_reactor(self) -> None:
+        subject = Subject()
+        with assert_not_reactor_called(subject.react['subject_method']):
+            Subject().react.trigger()
+
+    def test_instance_attribute_trigger_without_reactors(self) -> None:
+        Subject().react['subject_method'].react.trigger()
+
+    def test_instance_attribute_trigger_with_instance_reactor(self) -> None:
+        subject = Subject()
+        with assert_reactor_called(subject):
+            subject.react['subject_method'].react.trigger()
+
+    def test_instance_attribute_trigger_with_instance_attribute_reactor(self) -> None:
+        subject = Subject()
+        with assert_reactor_called(subject.react['subject_method']):
+            subject.react['subject_method'].react.trigger()
+
+
+class TestInstanceAttributeDefinition:
+    class InstanceAttributeDefinitionSubject(ReactiveInstance):
+        @reactive_method
+        def subject(self) -> None:
+            pass
+
+    class InheritedInstanceAttributeDefinitionSubject(InstanceAttributeDefinitionSubject):
+        pass
+
+    def test_iter_with_own_reactive_attribute(self) -> None:
+        assert 1 == len(list(InstanceAttributeDefinition.iter(self.InstanceAttributeDefinitionSubject, 'subject')))
+
+    def test_iter_with_inherited_reactive_attribute(self) -> None:
+        assert 1 == len(list(InstanceAttributeDefinition.iter(self.InheritedInstanceAttributeDefinitionSubject, 'subject')))
+
+    def test_iter_with_local_should_error(self) -> None:
+        class Local(ReactiveInstance):
+            pass
+
+        with pytest.raises(ValueError):
+            list(InstanceAttributeDefinition.iter(Local, 'local'))
+
+    def test_register_with_local_should_error(self) -> None:
+        def local() -> None:
+            pass
+        with pytest.raises(ValueError):
+            InstanceAttributeDefinition(local)
```

### Comparing `reactives-0.4.3/reactives/reactor.py` & `reactives-0.5.0/reactives/reactor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,269 @@
 from __future__ import annotations
+
 import copy
 import inspect
 import weakref
-from collections import deque
-from contextlib import contextmanager, suppress
-from typing import Sequence, Tuple, Optional, Dict, Set, Any, Iterator, cast, Callable, Union, List
-
-try:
-    from typing import Self  # type: ignore
-except ImportError:
-    from typing_extensions import Self  # type: ignore
+from _weakref import ReferenceType
+from collections import defaultdict
+from contextlib import suppress
+from enum import IntEnum, auto
+from typing import Tuple, Dict, Any, Iterator, Callable, Union, TypeVar, overload, MutableSequence, MutableMapping, cast
 
-from reactives.factory import Reactive
+from reactives import Reactive
 
 try:
     from graphlib import TopologicalSorter
-except ImportError:
-    from graphlib_backport import TopologicalSorter  # type: ignore
+except ImportError:  # pragma: no cover
+    from graphlib_backport import TopologicalSorter  # type: ignore[no-redef]  # pragma: no cover
+
+try:
+    from typing_extensions import Self, TypeAlias
+except ImportError:  # pragma: no cover
+    from typing import Self, TypeAlias  # type: ignore  # pragma: no cover
+
+
+class TriggerOrigin(IntEnum):
+    # A trigger originating from outside a reactive or reactor controller.
+    EXTERNAL = auto()
+    # A trigger originating from inside a reactor controller. This will skip the reactor controller's on-trigger event
+    # handler.
+    INTERNAL = auto()
+
+
+class _ReactorChain:
+    def __init__(self) -> None:
+        self._target_reactor_graph: MutableMapping[ReactorGraphNode, MutableSequence[ReactorGraphNode]] = defaultdict(list)
+        self._target_nodes: Iterator[ReactorGraphNode] | None = None
+
+    def update(
+            self,
+            source_reactor_controller: ReactorController,
+            origin: TriggerOrigin = TriggerOrigin.EXTERNAL,
+    ) -> None:
+        self._target_nodes = None
+        for source_reactor, target_reactor in self._resolve_edges(None, source_reactor_controller, origin):
+            if source_reactor is not None:
+                self._target_reactor_graph[target_reactor].append(source_reactor)
+
+    def _resolve_edges(
+            self,
+            source_node: ReactorGraphNode | None,
+            target_node: ReactorGraphNode,
+            origin: TriggerOrigin = TriggerOrigin.EXTERNAL,
+    ) -> Iterator[Tuple[ReactorGraphNode | None, ReactorGraphNode]]:
+        yield source_node, target_node
+        if isinstance(target_node, ReactorController):
+            yield from self._resolve_reactor_controller_edges(target_node, origin)
+
+    def _resolve_reactor_controller_edges(
+            self,
+            target_node: ReactorController,
+            origin: TriggerOrigin = TriggerOrigin.EXTERNAL,
+    ) -> Iterator[Tuple[ReactorGraphNode | None, ReactorGraphNode]]:
+        target_reactor_controller_reactors_source_node: ReactorGraphNode
+        if origin is TriggerOrigin.INTERNAL:
+            target_reactor_controller_reactors_source_node = target_node
+        else:
+            yield target_node, target_node._on_trigger
+            target_reactor_controller_reactors_source_node = target_node._on_trigger
+        for target_reactor_controller_reactor in target_node._reactors:
+            yield from self._resolve_edges(
+                target_reactor_controller_reactors_source_node,
+                target_reactor_controller_reactor,
+            )
+
+    def __iter__(self) -> Self:
+        return self
+
+    def __next__(self) -> Reactor:
+        # Rebuild the reactors if they were updated.
+        if self._target_nodes is None:
+            self._target_nodes = cast(Iterator[ReactorGraphNode], TopologicalSorter(self._target_reactor_graph).static_order())
+
+        target_reactor = next(self._target_nodes)
+
+        # Remove the reactor from the graph.
+        with suppress(KeyError):
+            del self._target_reactor_graph[target_reactor]
+        for source_reactors in self._target_reactor_graph.values():
+            with suppress(ValueError):
+                source_reactors.remove(target_reactor)
+
+        # Skip reactor controllers, which are kept for graph resolution, but are not reactors themselves.
+        if isinstance(target_reactor, ReactorController):
+            return self.__next__()
+        return target_reactor
+
+    def trigger(
+            self,
+            source_reactor_controller: ReactorController,
+            origin: TriggerOrigin = TriggerOrigin.EXTERNAL,
+    ) -> None:
+        self.update(source_reactor_controller, origin)
+        for target_reactor in self:
+            target_reactor()
+
+
+class _ReactorChainTrigger:
+    _current: _ReactorChain | None = None
+
+    @classmethod
+    def trigger(
+            cls,
+            source_reactor_controller: ReactorController,
+            origin: TriggerOrigin = TriggerOrigin.EXTERNAL,
+    ) -> None:
+        if cls._current:
+            cls._current.update(source_reactor_controller, origin)
+        else:
+            cls._current = _ReactorChain()
+            try:
+                cls._current.trigger(source_reactor_controller, origin)
+            finally:
+                cls._current = None
 
 
 class ReactorController:
-    _trigger_suspended: bool = False
-    _chain_is_reacting: bool = False
-    _chain_reactor_graph: Dict[Reactor, Set[Reactor]] = {}
-    _chain_reactors: deque = deque()
-    _chain_current_reactor: Optional[Reactor] = None
-
-    def __init__(self):
-        self._reactors = []
-        self._dependencies: List[Reactive] = []
+    def __init__(self) -> None:
+        self.__reactors: MutableSequence[ReactorGraphNode | ReferenceType[ReactorGraphNode]] = []
+        self._dependencies: MutableSequence[ReactorController] = []
 
-    def __call__(self, *args):
-        self.react(*args)
+    def __call__(self, *reactors: ResolvableReactor) -> None:
+        self.react(*reactors)
 
     def __copy__(self) -> Self:
         copied = self.__class__.__new__(self.__class__)
-        copied._reactors = copy.copy(self._reactors)
+        copied.__reactors = copy.copy(self.__reactors)
         return copied
 
     def __getstate__(self) -> Dict[str, Any]:
         return {
-            '_reactors': self._reactors,
+            '__reactors': self.__reactors,
+            '_dependencies': self._dependencies,
         }
 
     def __setstate__(self, state: Dict[str, Any]) -> None:
-        self._reactors = state['_reactors']
+        self.__reactors = state['__reactors']
+        self._dependencies = state['_dependencies']
 
     @property
-    def reactors(self) -> Sequence[Reactor]:
-        return [*self._reactors]
+    def _reactors(self) -> Iterator[ReactorGraphNode]:
+        yield from filter(None, map(
+            self._unweakref,  # type: ignore[arg-type]
+            self.__reactors,
+        ))
 
     def trigger(self) -> None:
-        if ReactorController._trigger_suspended:
-            return
+        _ReactorChainTrigger.trigger(self)
 
-        if self.trigger == ReactorController._chain_current_reactor:
-            return
-
-        self._update_reactor_graph()
-        self._trigger_reactor_chain()
-
-    def _update_reactor_graph(self) -> None:
-        if len(self._reactors) == 0:
-            return
+    def _trigger(self) -> None:
+        _ReactorChainTrigger.trigger(self, TriggerOrigin.INTERNAL)
 
-        for reactor in self._reactors:
-            for source_reactor, target_reactor in self._expand_reactor(None, reactor):
-                if target_reactor not in ReactorController._chain_reactor_graph:
-                    ReactorController._chain_reactor_graph[target_reactor] = set()
-                if source_reactor is not None:
-                    ReactorController._chain_reactor_graph[target_reactor].add(source_reactor)
-
-        ReactorController._chain_reactors = deque(TopologicalSorter(ReactorController._chain_reactor_graph).static_order())
-
-    def _expand_reactor(self, caller: Optional[Reactor], reactor: ResolvableReactor) -> Iterator[Tuple[Optional[Reactor], Reactor]]:
-        reactor = self._unweakref(reactor)
-
-        if isinstance(reactor, (ReactorController, Reactive)):
-            reactor_controller = resolve_reactor_controller(reactor)
-            yield caller, reactor_controller.trigger
-            for reactor_reactor in reactor_controller.reactors:
-                yield from self._expand_reactor(reactor_controller.trigger, reactor_reactor)
-        else:
-            yield caller, reactor
+    def _on_trigger(self) -> None:
+        pass
 
-    def _trigger_reactor_chain(self) -> None:
-        if ReactorController._chain_is_reacting:
-            return
-        ReactorController._chain_is_reacting = True
-        try:
-            while True:
-                try:
-                    ReactorController._chain_current_reactor = cast(Reactor, ReactorController._chain_reactors.popleft())
-                except IndexError:
-                    return
-
-                # Remove indegree vertices, if they exist. This keeps the graph as small as possible, allowing for the
-                # most efficient re-tsorting if it must be extended because of branched reactors.
-                with suppress(KeyError):
-                    del ReactorController._chain_reactor_graph[ReactorController._chain_current_reactor]
-
-                ReactorController._chain_current_reactor()
-        finally:
-            ReactorController._chain_is_reacting = False
-            ReactorController._chain_current_reactor = None
-
-    def _weakref(self, target, *args, **kwargs) -> weakref.ref:
-        if inspect.ismethod(target):
-            return weakref.WeakMethod(target, *args, **kwargs)
+    def _weakref(self, reactor: ReactorGraphNodeT, callback: Callable[[ReferenceType[ReactorGraphNodeT]], Any]) -> ReferenceType[ReactorGraphNodeT]:
+        if inspect.ismethod(reactor):
+            return weakref.WeakMethod(
+                reactor,  # type: ignore[arg-type]
+                callback,  # type: ignore[arg-type]
+            )
         # weakref.proxy is not hashable, so we use weakref.ref and dereference it ourselves.
-        return weakref.ref(target, *args, **kwargs)
+        return weakref.ref(reactor, callback)
 
-    def _unweakref(self, reference: Any) -> Any:
-        # weakref.proxy is not hashable, so we use weakref.ref and dereference it ourselves.
+    def _unweakref(self, reference: ReactorGraphNodeT | ReferenceType[ReactorGraphNodeT]) -> ReactorGraphNodeT | None:
         if isinstance(reference, weakref.ref):
             return reference()
         return reference
 
-    @classmethod
-    @contextmanager
-    def suspend(cls) -> Iterator[None]:
-        original_suspended = ReactorController._trigger_suspended
-        ReactorController._trigger_suspended = True
-        yield
-        ReactorController._trigger_suspended = original_suspended
+    def _resolve_reactor(self, reactor: ResolvableReactor) -> ReactorGraphNode:
+        if isinstance(reactor, Reactive):
+            return reactor.react
+        return reactor
+
+    def _append_reactor(self, reactor: ReactorGraphNode | ReferenceType[ReactorGraphNode]) -> None:
+        if reactor not in self.__reactors:
+            self.__reactors.append(reactor)
 
     def react(self, *reactors: ResolvableReactor) -> None:
         for reactor in reactors:
-            self._reactors.append(reactor)
+            self._append_reactor(self._resolve_reactor(reactor))
 
-    def shutdown(self, *reactors: ResolvableReactor) -> None:
-        from reactives import scope
+    def react_weakref(self, *reactors: ResolvableReactor) -> None:
+        for reactor in reactors:
+            self._append_reactor(self._weakref(self._resolve_reactor(reactor), self._shutdown_reactor))
 
+    def shutdown(self, *reactors: ResolvableReactor) -> None:
         if not reactors:
-            self._reactors.clear()
+            self.__reactors.clear()
             return
 
-        with scope.suspend():
-            for reactor in reactors:
-                self._shutdown_reactor(reactor)
+        for reactor in reactors:
+            self._shutdown_reactor(reactor)
 
     def _shutdown_reactor(self, reactor: ResolvableReactor) -> None:
-        # This is identical to self._reactors.remove(reactor), but we resolve weakrefs first.
+        reactor = self._resolve_reactor(reactor)
         # To prevent the list from reindexing the values we still have to remove, compare reactors in reverse.
-        for i, self_reactor in reversed(list(enumerate(map(self._unweakref, self._reactors)))):
+        for i, self_reactor in reversed(list(enumerate(map(
+            self._unweakref,  # type: ignore[arg-type]
+            self.__reactors,
+        )))):
             if reactor == self_reactor:
-                del self._reactors[i]
-                # Only delete the first occurrence, just like list.remove().
-                return
-
-    def react_weakref(self, *reactors: ResolvableReactor) -> None:
-        """
-        Add a reactor using a weakref.
-
-        This is a small helper, and it doesn't do much, but it serves as a reminder for people that it's important to
-        consider using weakrefs for the performance of their application: if a reactor is added without a weakref, it
-        MUST be shut down explicitly or a reference to it will exist forever, consuming memory and potentially slowing
-        down reactivity.
-        """
-        for reactor in reactors:
-            self.react(self._weakref(reactor, self._reactors.remove))
-
+                del self.__reactors[i]
 
-Reactor = Callable[[], Any]
 
+Reactor: TypeAlias = Callable[[], Any]
+ReactorGraphNode: TypeAlias = Union[Reactor, ReactorController]
+ReactorGraphNodeT = TypeVar('ReactorGraphNodeT', bound=ReactorGraphNode)
+ReactorControllerT = TypeVar('ReactorControllerT', bound=ReactorController)
+ResolvableReactorController: TypeAlias = Union[ReactorController, Reactive]
+ResolvableReactorControllerT = TypeVar('ResolvableReactorControllerT', bound=ResolvableReactorController)
+ResolvableReactor: TypeAlias = Union[Reactor, ResolvableReactorController]
+ResolvableReactorT = TypeVar('ResolvableReactorT', bound=ResolvableReactor)
 
-ResolvableReactor = Union[Reactor, ReactorController, Reactive]
 
+@overload
+def resolve_reactor_controller(resolvable: Reactive) -> ReactorController:
+    pass
 
-def resolve_reactor(reactor: ResolvableReactor) -> Iterator[Reactor]:
-    if isinstance(reactor, (ReactorController, Reactive)):
-        yield from resolve_reactor_controller(reactor).reactors
-        return
-    yield reactor
 
+@overload
+def resolve_reactor_controller(resolvable: ReactorController) -> ReactorController:
+    pass
 
-ResolvableReactorController = Union[ReactorController, Reactive]
 
-
-def resolve_reactor_controller(reactor_controller: ResolvableReactorController) -> ReactorController:
-    if isinstance(reactor_controller, Reactive):
-        return reactor_controller.react
-    return reactor_controller
+def resolve_reactor_controller(resolvable: ResolvableReactorController) -> ReactorController:
+    if isinstance(resolvable, ReactorController):
+        return resolvable
+    if isinstance(resolvable, Reactive):
+        return resolvable.react
+    raise ValueError(f'Cannot resolve the reactor controller for {resolvable}.')  # pragma: no cover
 
 
 ExpectedCallCount = Union[int, Tuple[int, int], Tuple[int, None], Tuple[None, int]]
 
 
 class AssertCallCountReactor:
-    def __init__(self, expected_call_count: ExpectedCallCount):
-        self._exact_expected_call_count: Optional[int]
-        self._minimum_expected_call_count: Optional[int]
-        self._maximum_expected_call_count: Optional[int]
+    def __init__(self, reactor_controller: ReactorController, expected_call_count: ExpectedCallCount = 1):
+        self._exact_expected_call_count: int | None
+        self._minimum_expected_call_count: int | None
+        self._maximum_expected_call_count: int | None
         if isinstance(expected_call_count, int):
             self._exact_expected_call_count = expected_call_count
             self._minimum_expected_call_count = expected_call_count
             self._maximum_expected_call_count = expected_call_count
         else:
             self._exact_expected_call_count = None
             self._minimum_expected_call_count, self._maximum_expected_call_count = expected_call_count
         self._actual_call_count = 0
+        self._reactor_controller = reactor_controller
+
+    def __repr__(self) -> str:
+        return f'<{self.__class__.__module__}.{self.__class__.__qualname__} object at {hex(id(self))} for {repr(self._reactor_controller)}>'
 
     def __call__(self) -> None:
         self._actual_call_count += 1
         self._assert_maximum_call_count()
 
     def _assert(self, expectation_message: str) -> None:
         raise AssertionError(f'Failed asserting that a reactor ({self}) was {expectation_message}. Instead, it was actually called {self._actual_call_count} time(s).')
```

### Comparing `reactives-0.4.3/reactives/tests/__init__.py` & `reactives-0.5.0/reactives/tests/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,58 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import Union, Iterator, Optional, overload, Any, ContextManager
+from typing import Iterator, Any
 
-from reactives import scope
-from reactives.factory import Reactive
+from reactives import scope, Reactive
 from reactives.reactor import Reactor, ReactorController, ResolvableReactorController, resolve_reactor_controller, \
     AssertCallCountReactor, ExpectedCallCount
 
 
 class _DummyReactive(Reactive):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.react = ReactorController()
 
 
-@overload
-def _assert_reactor(reactor: Reactor, sut: None = None) -> Iterator[Reactor]:
-    pass
-
-
-@overload
 def _assert_reactor(reactor: Reactor, sut: ResolvableReactorController) -> Iterator[None]:
-    pass
-
-
-def _assert_reactor(reactor: Reactor, sut: Optional[ResolvableReactorController] = None) -> Iterator[Optional[Reactor]]:
-    if sut is not None:
-        sut = resolve_reactor_controller(sut)
-        sut.react(reactor)
+    sut = resolve_reactor_controller(sut)
+    sut.react(reactor)
+    try:
         yield None
+    finally:
         sut.shutdown(reactor)
-    else:
-        yield reactor
-
-
-@overload
-def assert_reactor_called(expected_call_count: ExpectedCallCount = 1) -> ContextManager[Reactor]:
-    pass
-
-
-@overload
-def assert_reactor_called(sut: Union[Reactive, ReactorController], expected_call_count: ExpectedCallCount = 1) -> ContextManager[None]:
-    pass
 
 
 # Ignore the decorator because Mypy falsely flags it as a type violation (https://github.com/python/mypy/issues/11373).
-@contextmanager  # type: ignore
-def assert_reactor_called(sut: Any = None, expected_call_count: ExpectedCallCount = 1) -> Iterator[Optional[Reactor]]:
-    reactor = AssertCallCountReactor(expected_call_count)
-    yield from _assert_reactor(reactor, sut)
+@contextmanager  # type: ignore[misc]
+def assert_reactor_called(reactor_controller: ResolvableReactorController, expected_call_count: ExpectedCallCount = 1) -> Iterator[None]:
+    reactor_controller = resolve_reactor_controller(reactor_controller)
+    reactor = AssertCallCountReactor(reactor_controller, expected_call_count)
+    yield from _assert_reactor(reactor, reactor_controller)
     reactor.assert_call_count()
 
 
-@overload
-def assert_not_reactor_called() -> ContextManager[Reactor]:
-    pass
-
-
-@overload
-def assert_not_reactor_called(sut: ResolvableReactorController) -> ContextManager[None]:
-    pass
-
-
-@contextmanager  # type: ignore
-def assert_not_reactor_called(sut: Optional[ResolvableReactorController] = None) -> Iterator[Optional[Reactor]]:
-    yield from _assert_reactor(AssertCallCountReactor(0), sut)
+# Ignore the decorator because Mypy falsely flags it as a type violation (https://github.com/python/mypy/issues/11373).
+@contextmanager  # type: ignore[misc]
+def assert_not_reactor_called(reactor_controller: ResolvableReactorController) -> Iterator[None]:
+    reactor_controller = resolve_reactor_controller(reactor_controller)
+    yield from _assert_reactor(AssertCallCountReactor(reactor_controller, 0), reactor_controller)
 
 
 @contextmanager
 def assert_scope_empty() -> Iterator[None]:
     reactive = _DummyReactive()
     with scope.collect(reactive):
         yield
     if reactive.react._dependencies:
         raise AssertionError(f'Failed asserting that the reactive scope is empty. Instead it is: {reactive.react._dependencies}')
 
 
 @contextmanager
-def assert_in_scope(dependency: Reactive) -> Iterator[None]:
+def assert_in_scope(*dependencies: ResolvableReactorController) -> Iterator[None]:
     reactive = _DummyReactive()
     with scope.collect(reactive):
         yield
-    if dependency not in reactive.react._dependencies:
-        raise AssertionError(f'Failed asserting that {dependency} was added to the reactive scope.')
+    for dependency in dependencies:
+        if resolve_reactor_controller(dependency) not in reactive.react._dependencies:
+            raise AssertionError(f'Failed asserting that {dependency} was added to the reactive scope.')
```

### Comparing `reactives-0.4.3/reactives/tests/factory/test_function.py` & `reactives-0.5.0/reactives/tests/instance/test_method.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,124 +1,102 @@
-import copy
-import pickle
-from unittest import TestCase
-
-from reactives import reactive
-from reactives.factory.function import _FunctionReactorController
-from reactives.factory.type import ReactiveInstance
+from reactives.function import reactive_function
+from reactives.instance import ReactiveInstance
+from reactives.instance.method import reactive_method
 from reactives.tests import assert_reactor_called, assert_not_reactor_called
 
 
-class ReactiveFunctionControllerTest(TestCase):
-    def test___copy__(self) -> None:
-        @reactive
-        def subject():
-            pass
-        sut = _FunctionReactorController()
-        with assert_reactor_called(sut):
-            copied_sut = copy.copy(sut)
-            with assert_not_reactor_called(sut):
-                with assert_reactor_called(copied_sut):
-                    copied_sut.trigger()
-
-    @reactive
-    class _Reactive(ReactiveInstance):
-        @reactive
-        def subject(self) -> None:
-            pass
-
-    def test___getstate__(self) -> None:
-        subject = self._Reactive()
-        # Call the function so the instance can lazily instantiate the reactor controller we are testing here.
-        subject.subject()
-        unpickled_subject = pickle.loads(pickle.dumps(subject))
-        with assert_not_reactor_called(subject):
-            with assert_reactor_called(unpickled_subject):
-                unpickled_subject.react['subject'].react.trigger()
-
-
-class ReactiveFunctionTest(TestCase):
-    def test_without_reactors(self) -> None:
-        @reactive
-        def subject():
-            subject.tracker.append(True)
-        subject.tracker = []
-        subject()
-        self.assertEqual([True], subject.tracker)
-
-    def test_with_reactor(self) -> None:
-        @reactive
-        def subject():
-            raise AssertionError('This function should not have been called.')
-
-        with assert_reactor_called(subject):
-            subject.react.trigger()
-
-    def test_with_reactor_and_dependency(self) -> None:
-        @reactive
-        def dependency():
-            pass
-
-        @reactive
-        def subject():
-            if not subject.called:
-                subject.called = True
-                dependency()
-        subject.called = False
-        with assert_reactor_called(subject):
-            # Call the reactive for the first time. This should result in dependency() being autowired.
-            subject()
-            # dependency() being autowired should cause the reactor to be called.
-            dependency.react.trigger()
-
-            # Call the reactive again. This should result in dependency() being ignored and not to be autowired again.
-            subject()
-            # dependency() no longer being autowired should not cause the reactor to be called.
-            dependency.react.trigger()
-
-    def test_with_reactor_and_dependency_as_instance_method(self) -> None:
-        @reactive
-        def dependency():
-            pass
-
-        @reactive
-        class Subject(ReactiveInstance):
-            def __init__(self):
-                self.called = False
-
-            @reactive
-            def subject(self):
-                if not self.called:
-                    self.called = True
-                    dependency()
+@reactive_function
+def dependency_one() -> None:
+    dependency_two()
+
+
+@reactive_function
+def dependency_two() -> None:
+    pass
+
+
+class Subject(ReactiveInstance):
+    @reactive_method
+    def subject(self, call_dependency: bool) -> None:
+        if call_dependency:
+            dependency_one()
+
+
+class SubjectWithOnTriggerCall(ReactiveInstance):
+    def __init__(self) -> None:
+        super().__init__()
+        self.on_trigger_calls = 0
+
+    @reactive_method(on_trigger_call=True)
+    def subject(self) -> None:
+        self.on_trigger_calls += 1
+
+
+class TestReactiveMethod:
+    def test_wrapped_metadata_for_class_method(self) -> None:
+        assert 'reactives.tests.instance.test_method' == Subject.subject.__module__
+        assert 'subject' == Subject.subject.__name__
+        assert 'Subject.subject' == Subject.subject.__qualname__
+
+    def test_wrapped_metadata_for_instance_method(self) -> None:
+        assert 'reactives.tests.instance.test_method' == Subject().subject.__module__
+        assert 'subject' == Subject().subject.__name__
+        assert 'Subject.subject' == Subject().subject.__qualname__
+
+    def test_call_as_class_method(self) -> None:
         subject = Subject()
-        with assert_reactor_called(subject):
-            # Call the reactive for the first time. This should result in dependency() being autowired.
-            subject.subject()
-            # dependency() being autowired should cause the reactor to be called.
-            dependency.react.trigger()
-
-            # Call the reactive again. This should result in dependency() being ignored and not to be autowired again.
-            subject.subject()
-            # dependency() no longer being autowired should not cause the reactor to be called.
-            dependency.react.trigger()
-
-    def test_on_trigger_call(self):
-        @reactive(on_trigger_call=True)
-        def subject():
-            subject.tracker.append(True)
-        subject.tracker = []
-        subject.react.trigger()
-        self.assertEqual([True], subject.tracker)
-
-    def test_on_trigger_call_as_instance_method(self):
-        @reactive
-        class Subject(ReactiveInstance):
-            def __init__(self):
-                self.tracker = []
-
-            @reactive(on_trigger_call=True)
-            def subject(self):
-                self.tracker.append(True)
+
+        # Call the reactive for the first time. This should result in dependency_one() being autowired to
+        # subject.subject()
+        Subject.subject(subject, True)
+
+        # dependency_one() being autowired to subject.subject() should cause subject.subject() to be triggered.
+        with assert_reactor_called(subject.react['subject']):
+            dependency_one.react.trigger()
+
+        # dependency_two() being autowired to dependency_one() should cause subject.subject() and dependency_one() to be
+        # triggered.
+        with assert_reactor_called(subject.react['subject']):
+            with assert_reactor_called(dependency_one):
+                dependency_two.react.trigger()
+
+        # Ensure that dependencies are only added to the direct calling scope, and not to ancestors' scopes.
+        assert dependency_one.react in list(dependency_two.react._reactors)
+
+        # Call the reactive again. This should result in dependency() being ignored and not to be autowired again.
+        Subject.subject(subject, False)
+
+        # dependency_one() no longer being autowired should not cause subject.subject() to be triggered.
+        with assert_not_reactor_called(subject.react['subject']):
+            dependency_one.react.trigger()
+
+    def test_call_as_instance_method(self) -> None:
         subject = Subject()
+
+        # Call the reactive for the first time. This should result in dependency_one() being autowired to
+        # subject.subject()
+        subject.subject(True)
+
+        # dependency_one() being autowired to subject.subject() should cause subject.subject() to be triggered.
+        with assert_reactor_called(subject.react['subject']):
+            dependency_one.react.trigger()
+
+        # dependency_two() being autowired to dependency_one() should cause subject.subject() and dependency_one() to be
+        # triggered.
+        with assert_reactor_called(subject.react['subject']):
+            with assert_reactor_called(dependency_one):
+                dependency_two.react.trigger()
+
+        # Ensure that dependencies are only added to the direct calling scope, and not to ancestors' scopes.
+        assert dependency_one.react in list(dependency_two.react._reactors)
+
+        # Call the reactive again. This should result in dependency() being ignored and not to be autowired again.
+        subject.subject(False)
+
+        # dependency_one() no longer being autowired should not cause subject.subject() to be triggered.
+        with assert_not_reactor_called(subject.react['subject']):
+            dependency_one.react.trigger()
+
+    def test_on_trigger_call(self) -> None:
+        subject = SubjectWithOnTriggerCall()
         subject.react['subject'].react.trigger()
-        self.assertEqual([True], subject.tracker)
+        assert subject.on_trigger_calls == 1
```

### Comparing `reactives-0.4.3/reactives/tests/test_collections.py` & `reactives-0.5.0/reactives/tests/test_collections.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,601 +1,602 @@
+from __future__ import annotations
+
 import copy
+from typing import Union, TYPE_CHECKING, Iterable, Tuple
+
 import dill as pickle
-import sys
-import unittest
-from unittest import TestCase
-
-from reactives import reactive
-from reactives.collections import ReactiveList, ReactiveDict
-from reactives.factory.type import ReactiveInstance
+
+from reactives import Reactive
+from reactives.collections import ReactiveMapping, ReactiveMutableMapping, ReactiveSequence, ReactiveMutableSequence
+from reactives.reactor import ReactorController
 from reactives.tests import assert_scope_empty, assert_reactor_called, assert_in_scope, assert_not_reactor_called
 
+if TYPE_CHECKING:
+    from _typeshed import SupportsKeysAndGetItem
+
 
-@reactive
-class _Reactive(ReactiveInstance):
-    pass
+class _Reactive(Reactive):
+    def __init__(self) -> None:
+        super().__init__()
+        self.react = ReactorController()
 
 
-class ReactiveDictTest(TestCase):
+class TestReactiveMapping:
     def test___getstate__(self) -> None:
         value = _Reactive()
-        subject = ReactiveDict(value=value)
-        copied_subject = pickle.loads(pickle.dumps(subject))
-        copied_value = copied_subject['value']
+        sut = ReactiveMapping[str, Reactive](value=value)
+        copied_sut = pickle.loads(pickle.dumps(sut))
+        copied_value = copied_sut['value']
 
         # Assert that the copy contains exactly one value which is a copy of the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIsNot(value, copied_value)
+        assert 1 == len(copied_sut)
+        assert value != copied_value
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that neither the copied instance nor the copied value is triggered when triggering the original value.
-        with assert_not_reactor_called(copied_subject):
+        with assert_not_reactor_called(copied_sut):
             with assert_not_reactor_called(copied_value):
-                with assert_reactor_called(subject):
+                with assert_reactor_called(sut):
                     with assert_reactor_called(value):
                         value.react.trigger()
 
         # Assert that neither the original instance nor the original value is triggered when triggering the copied
         # value.
-        with assert_not_reactor_called(subject):
+        with assert_not_reactor_called(sut):
             with assert_not_reactor_called(value):
-                with assert_reactor_called(copied_subject):
+                with assert_reactor_called(copied_sut):
                     with assert_reactor_called(copied_value):
                         copied_value.react.trigger()
 
     def test___copy__(self) -> None:
         value = _Reactive()
-        subject = ReactiveDict(value=value)
-        copied_subject = copy.copy(subject)
+        sut = ReactiveMapping[str, Reactive](value=value)
+        copied_sut = copy.copy(sut)
 
         # Assert that the copy contains exactly the same values as the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIs(value, copied_subject['value'])
+        assert 1 == len(copied_sut)
+        assert value is copied_sut['value']
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that triggering the value triggers both the original and the copy.
-        with assert_reactor_called(value):
-            with assert_reactor_called(copied_subject):
+        with assert_reactor_called(copied_sut):
+            with assert_reactor_called(sut):
                 value.react.trigger()
 
     def test___deepcopy__(self) -> None:
         value = _Reactive()
-        subject = ReactiveDict(value=value)
-        copied_subject = copy.deepcopy(subject)
-        copied_value = copied_subject['value']
+        sut = ReactiveMapping[str, Reactive](value=value)
+        copied_sut = copy.deepcopy(sut)
+        copied_value = copied_sut['value']
 
         # Assert that the copy contains exactly one value which is a copy of the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIsNot(value, copied_value)
+        assert 1 == len(copied_sut)
+        assert value is not copied_value
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that neither the copied instance nor the copied value is triggered when triggering the original value.
-        with assert_not_reactor_called(copied_subject):
+        with assert_not_reactor_called(copied_sut):
             with assert_not_reactor_called(copied_value):
-                with assert_reactor_called(subject):
-                    with assert_reactor_called(value):
-                        value.react.trigger()
+                with assert_reactor_called(sut):
+                    value.react.trigger()
 
         # Assert that neither the original instance nor the original value is triggered when triggering the copied
         # value.
-        with assert_not_reactor_called(subject):
+        with assert_not_reactor_called(sut):
             with assert_not_reactor_called(value):
-                with assert_reactor_called(copied_subject):
+                with assert_reactor_called(copied_sut):
                     with assert_reactor_called(copied_value):
                         copied_value.react.trigger()
 
-    def test_clear(self) -> None:
-        reactive_value = _Reactive()
-        sut = ReactiveDict(one=1, reactive=reactive_value)
-        with assert_scope_empty():
-            with assert_reactor_called(sut):
-                sut.clear()
-        self.assertCountEqual([], sut)
-        self.assertCountEqual([], reactive_value.react._reactors)
-
     def test_get(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert 2 == sut.get('two')
+
+    def test_get_with_default(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
         with assert_in_scope(sut):
-            self.assertEqual(2, sut.get('two'))
+            assert 3 == sut.get('three', 3)
 
     def test_items(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
+        sut = ReactiveMapping[str, int](one=1, two=2)
         with assert_in_scope(sut):
-            self.assertEqual([('one', 1), ('two', 2)], list(sut.items()))
+            assert [('one', 1), ('two', 2)] == list(sut.items())
 
     def test_keys(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert ['one', 'two'] == list(sut.keys())
+
+    def test_values(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert {'one': 1, 'two': 2} == dict(sut.items())
+
+    def test_contains(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert 'one' in sut
+            assert 'three' not in sut
+
+    def test_eq(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert {
+                'one': 1,
+                'two': 2,
+            } == sut
+
+    def test_getitem(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert 2 == sut['two']
+
+    def test_iter(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert ['one', 'two'] == list(iter(sut))
+
+    def test_len(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert 2 == len(sut)
+
+    def test_ne(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
         with assert_in_scope(sut):
-            self.assertEqual(['one', 'two'], list(sut.keys()))
+            assert {
+                'two': 1,
+                'one': 2,
+            } != sut
+
+    def test_reversed(self) -> None:
+        sut = ReactiveMapping[str, int](one=1, two=2)
+        with assert_in_scope(sut):
+            assert ['two', 'one'] == list(reversed(sut))
+
+
+class TestReactiveMutableMapping:
+    def test_clear(self) -> None:
+        reactive_value = _Reactive()
+        sut = ReactiveMutableMapping[str, Union[Reactive, int]](one=1, reactive=reactive_value)
+        with assert_scope_empty():
+            with assert_reactor_called(sut):
+                sut.clear()
+        assert {} == dict(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
     def test_pop(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict(reactive=reactive_value)
+        sut = ReactiveMutableMapping[str, Reactive](reactive=reactive_value)
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.pop('reactive')
-        self.assertCountEqual([], sut)
-        self.assertCountEqual([], reactive_value.react._reactors)
+        assert {} == dict(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
+
+    def test_pop_with_default(self) -> None:
+        reactive_value = _Reactive()
+        sut = ReactiveMutableMapping[str, Reactive](reactive=reactive_value)
+        with assert_scope_empty():
+            with assert_reactor_called(sut):
+                assert 3 == sut.pop('three', 3)
+        assert dict(reactive=reactive_value) == dict(sut)
 
     def test_popitem(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict(reactive=reactive_value)
+        sut = ReactiveMutableMapping[str, Reactive](reactive=reactive_value)
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 key, value = sut.popitem()
-        self.assertEqual('reactive', key)
-        self.assertEqual(reactive_value, value)
-        self.assertCountEqual([], sut)
-        self.assertCountEqual([], reactive_value.react._reactors)
+        assert 'reactive' == key
+        assert reactive_value == value
+        assert {} == dict(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
     def test_setdefault_with_existing_key(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict(reactive='notActuallyReactive')
+        sut = ReactiveMutableMapping[str, Union[Reactive, str]](reactive=reactive_value)
         with assert_in_scope(sut):
             with assert_not_reactor_called(sut):
-                sut.setdefault('reactive', reactive_value)
-        self.assertNotEqual(reactive_value, dict.get(sut, 'reactive'))
-        self.assertNotIn(sut, reactive_value.react._reactors)
+                assert reactive_value == sut.setdefault('reactive')
 
     def test_setdefault_with_unknown_key(self) -> None:
-        reactive_value = _Reactive()
-        sut = ReactiveDict()
+        sut = ReactiveMutableMapping[str, Reactive]()
         with assert_in_scope(sut):
             with assert_reactor_called(sut):
+                assert sut.setdefault('reactive') is None
+        assert sut['reactive'] is None
+
+    def test_setdefault_with_existing_key_with_value(self) -> None:
+        reactive_value = _Reactive()
+        sut = ReactiveMutableMapping[str, Union[Reactive, str]](reactive='notActuallyReactive')
+        with assert_in_scope(sut):
+            with assert_not_reactor_called(sut):
                 sut.setdefault('reactive', reactive_value)
-        self.assertEqual(reactive_value, dict.get(sut, 'reactive'))
-        self.assertIn(sut, reactive_value.react._reactors)
+        assert reactive_value != sut['reactive']
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
-    def test_update(self) -> None:
+    def test_setdefault_with_unknown_key_with_value(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict(one=1)
-        with assert_scope_empty():
+        sut = ReactiveMutableMapping[str, Reactive]()
+        with assert_in_scope(sut):
             with assert_reactor_called(sut):
-                sut.update({
-                    'reactive': reactive_value
-                })
-        self.assertEqual(reactive_value, dict.get(sut, 'reactive'))
-        self.assertIn(sut, reactive_value.react._reactors)
+                sut.setdefault('reactive', reactive_value)
+        assert reactive_value == sut['reactive']
+        with assert_reactor_called(sut):
+            reactive_value.react.trigger()
 
-    def test_values(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertCountEqual([1, 2], list(sut.values()))
+    def test_update_with_supports_keys_and_get_item(self) -> None:
+        reactive_value_1 = _Reactive()
+        reactive_value_2 = _Reactive()
+        sut = ReactiveMutableMapping[str, Union[Reactive, int]](reactive_1=reactive_value_1)
+        update_value: SupportsKeysAndGetItem = {
+            'reactive_2': reactive_value_2,
+            'two': 2,
+        }
+        with assert_scope_empty():
+            with assert_reactor_called(sut):
+                sut.update(update_value)
+        assert {
+            'reactive_1': reactive_value_1,
+            'reactive_2': reactive_value_2,
+            'two': 2,
+        } == dict(sut)
+        with assert_reactor_called(sut):
+            reactive_value_1.react.trigger()
+        with assert_reactor_called(sut):
+            reactive_value_2.react.trigger()
 
-    def test_contains(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertIn('one', sut)
-            self.assertNotIn('three', sut)
+    def test_update_with_iterable(self) -> None:
+        reactive_value_1 = _Reactive()
+        reactive_value_2 = _Reactive()
+        sut = ReactiveMutableMapping[str, Union[Reactive, int]](reactive_1=reactive_value_1)
+        update_value: Iterable[Tuple[str, Union[Reactive, int]]] = [
+            ('reactive_2', reactive_value_2),
+            ('two', 2),
+        ]
+        with assert_scope_empty():
+            with assert_reactor_called(sut):
+                sut.update(update_value)
+        assert {
+            'reactive_1': reactive_value_1,
+            'reactive_2': reactive_value_2,
+            'two': 2,
+        } == dict(sut)
+        with assert_reactor_called(sut):
+            reactive_value_1.react.trigger()
+        with assert_reactor_called(sut):
+            reactive_value_2.react.trigger()
+
+    def test_update_with_kwargs(self) -> None:
+        reactive_value_1 = _Reactive()
+        reactive_value_2 = _Reactive()
+        sut = ReactiveMutableMapping[str, Union[Reactive, int]](reactive_1=reactive_value_1)
+        with assert_scope_empty():
+            with assert_reactor_called(sut):
+                sut.update(reactive_2=reactive_value_2, two=2)
+        assert {
+            'reactive_1': reactive_value_1,
+            'reactive_2': reactive_value_2,
+            'two': 2,
+        } == dict(sut)
+        with assert_reactor_called(sut):
+            reactive_value_1.react.trigger()
+        with assert_reactor_called(sut):
+            reactive_value_2.react.trigger()
 
     def test_delitem(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict(reactive=reactive_value)
+        sut = ReactiveMutableMapping[str, Reactive](reactive=reactive_value)
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 del sut['reactive']
-        self.assertCountEqual([], sut)
-        self.assertCountEqual([], reactive_value.react._reactors)
-
-    def test_eq(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertEqual({
-                'one': 1,
-                'two': 2,
-            }, sut)
-
-    def test_getitem(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertEqual(2, sut['two'])
-
-    def test_iter(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertCountEqual(['one', 'two'], iter(sut))
-
-    def test_len(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertEqual(2, len(sut))
-
-    def test_ne(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            self.assertNotEqual({
-                'two': 1,
-                'one': 2,
-            }, sut)
-
-    @unittest.skipIf(not hasattr(dict, '__reversed__'), 'Dictionary reversal is available in Python 3.8 and later only.')
-    def test_reversed(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            # Because dictionary order isn't guaranteed before Python 3.7, we cannot compare to a hardcoded list of
-            # expected keys.
-            self.assertEqual(['two', 'one'], list(reversed(sut)))
+        assert {} == dict(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
     def test_setitem(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveDict()
+        sut = ReactiveMutableMapping[str, Reactive]()
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut['reactive'] = reactive_value
-        self.assertEqual(reactive_value, sut['reactive'])
+        assert reactive_value == sut['reactive']
         with assert_reactor_called(sut):
             reactive_value.react.trigger()
 
-    def test_sizeof(self) -> None:
-        sut = ReactiveDict(one=1, two=2)
-        with assert_in_scope(sut):
-            sys.getsizeof(sut)
-
 
-class ReactiveListTest(TestCase):
+class TestReactiveSequence:
     def test___getstate__(self) -> None:
         value = _Reactive()
-        subject = ReactiveList([value])
-        copied_subject = pickle.loads(pickle.dumps(subject))
-        copied_value = copied_subject[0]
+        sut = ReactiveSequence[Reactive]([value])
+        copied_sut = pickle.loads(pickle.dumps(sut))
+        copied_value = copied_sut[0]
 
         # Assert that the copy contains exactly one value which is a copy of the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIsNot(value, copied_value)
+        assert 1 == len(copied_sut)
+        assert value is not copied_value
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that neither the copied instance nor the copied value is triggered when triggering the original value.
-        with assert_not_reactor_called(copied_subject):
+        with assert_not_reactor_called(copied_sut):
             with assert_not_reactor_called(copied_value):
-                with assert_reactor_called(subject):
+                with assert_reactor_called(sut):
                     with assert_reactor_called(value):
                         value.react.trigger()
 
         # Assert that neither the original instance nor the original value is triggered when triggering the copied
         # value.
-        with assert_not_reactor_called(subject):
+        with assert_not_reactor_called(sut):
             with assert_not_reactor_called(value):
-                with assert_reactor_called(copied_subject):
+                with assert_reactor_called(copied_sut):
                     with assert_reactor_called(copied_value):
                         copied_value.react.trigger()
 
     def test___copy__(self) -> None:
         value = _Reactive()
-        subject = ReactiveList([value])
-        copied_subject = copy.copy(subject)
-
-        # Assert that the copy contains exactly the same values as the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIs(value, copied_subject[0])
-
-        # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
-
-        # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
-
-        # Assert that triggering the value triggers both the original and the copy.
-        with assert_reactor_called(value):
-            with assert_reactor_called(copied_subject):
-                value.react.trigger()
-
-    def test_copy(self) -> None:
-        value = _Reactive()
-        subject = ReactiveList([value])
-        copied_subject = subject.copy()
+        sut = ReactiveSequence[Reactive]([value])
+        copied_sut = copy.copy(sut)
 
         # Assert that the copy contains exactly the same values as the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIs(value, copied_subject[0])
+        assert 1 == len(copied_sut)
+        assert value is copied_sut[0]
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that triggering the value triggers both the original and the copy.
         with assert_reactor_called(value):
-            with assert_reactor_called(copied_subject):
+            with assert_reactor_called(copied_sut):
                 value.react.trigger()
 
     def test___deepcopy__(self) -> None:
         value = _Reactive()
-        subject = ReactiveList([value])
-        copied_subject = copy.deepcopy(subject)
-        copied_value = copied_subject[0]
+        sut = ReactiveSequence[Reactive]([value])
+        copied_sut = copy.deepcopy(sut)
+        copied_value = copied_sut[0]
 
         # Assert that the copy contains exactly one value which is a copy of the original.
-        self.assertEqual(1, len(copied_subject))
-        self.assertIsNot(value, copied_value)
+        assert 1 == len(copied_sut)
+        assert value is not copied_value
 
         # Assert that triggering the original does not trigger the copy.
-        with assert_not_reactor_called(copied_subject):
-            subject.react.trigger()
+        with assert_not_reactor_called(copied_sut):
+            sut.react.trigger()
 
         # Assert that triggering the copy does not trigger the original.
-        with assert_not_reactor_called(subject):
-            copied_subject.react.trigger()
+        with assert_not_reactor_called(sut):
+            copied_sut.react.trigger()
 
         # Assert that neither the copied instance nor the copied value is triggered when triggering the original value.
-        with assert_not_reactor_called(copied_subject):
+        with assert_not_reactor_called(copied_sut):
             with assert_not_reactor_called(copied_value):
-                with assert_reactor_called(subject):
+                with assert_reactor_called(sut):
                     with assert_reactor_called(value):
                         value.react.trigger()
 
         # Assert that neither the original instance nor the original value is triggered when triggering the copied
         # value.
-        with assert_not_reactor_called(subject):
+        with assert_not_reactor_called(sut):
             with assert_not_reactor_called(value):
-                with assert_reactor_called(copied_subject):
+                with assert_reactor_called(copied_sut):
                     with assert_reactor_called(copied_value):
                         copied_value.react.trigger()
 
+    def test_count(self) -> None:
+        sut = ReactiveSequence[int]([1, 2, 1])
+        with assert_in_scope(sut):
+            assert 2 == sut.count(1)
+
+    def test_index_without_slice(self) -> None:
+        sut = ReactiveSequence[int]([1, 2, 1, 2, 1, 2, 1, 2])
+        with assert_in_scope(sut):
+            assert 1 == sut.index(2)
+
+    def test_index_with_slice(self) -> None:
+        sut = ReactiveSequence[int]([1, 2, 1, 2, 1, 2, 1, 2])
+        with assert_in_scope(sut):
+            assert 2 == sut.index(1, 2, 5)
+
+    def test_contains(self) -> None:
+        sut = ReactiveSequence[int]([1])
+        with assert_in_scope(sut):
+            assert 1 in sut
+            assert 2 not in sut
+
+    def test___getitem_with_int(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert 2 == sut[1]
+
+    def test___getitem_with_slice(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert [1, 2] == list(sut[0:2])
+
+    def test_iter(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert [1, 2] == list(iter(sut))
+
+    def test_len(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert 2 == len(sut)
+
+    def test_ne(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert [2, 1] != list(sut)
+
+    def test_reversed(self) -> None:
+        sut = ReactiveSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert [2, 1] == list(reversed(sut))
+
+
+class TestReactiveMutableSequence:
     def test_append(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList()
+        sut = ReactiveMutableSequence[Reactive]()
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.append(reactive_value)
         with assert_reactor_called(sut):
             reactive_value.react.trigger()
 
     def test_clear(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([reactive_value])
+        sut = ReactiveMutableSequence[Reactive]([reactive_value])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.clear()
-        self.assertEqual([], sut)
-        self.assertEqual([], reactive_value.react._reactors)
-
-    def test_count(self) -> None:
-        sut = ReactiveList([1, 2, 1])
-        with assert_in_scope(sut):
-            self.assertEqual(2, sut.count(1))
+        assert [] == list(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
     def test_extend(self) -> None:
         reactive_value1 = _Reactive()
         reactive_value2 = _Reactive()
-        sut = ReactiveList([1, 2])
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1, 2])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.extend([reactive_value1, reactive_value2])
-        self.assertEqual([1, 2, reactive_value1, reactive_value2], sut)
+        assert [1, 2, reactive_value1, reactive_value2] == list(sut)
         with assert_reactor_called(sut):
             reactive_value1.react.trigger()
         with assert_reactor_called(sut):
             reactive_value2.react.trigger()
 
-    def test_index_without_slice(self) -> None:
-        sut = ReactiveList([1, 2, 1, 2, 1, 2, 1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual(1, sut.index(2))
-
-    def test_index_with_slice(self) -> None:
-        sut = ReactiveList([1, 2, 1, 2, 1, 2, 1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual(2, sut.index(1, 2, 5))
-
     def test_insert(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([1, 2])
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1, 2])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.insert(1, reactive_value)
-        self.assertEqual([1, reactive_value, 2], sut)
+        assert [1, reactive_value, 2] == list(sut)
         with assert_reactor_called(sut):
             reactive_value.react.trigger()
 
     def test_pop_without_index(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([1, 2, reactive_value])
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1, 2, reactive_value])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.pop()
-        self.assertEqual([1, 2], sut)
+        assert [1, 2] == list(sut)
         with assert_not_reactor_called(sut):
             reactive_value.react.trigger()
 
     def test_pop_with_index(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([1, reactive_value, 2])
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1, reactive_value, 2])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.pop(1)
-        self.assertEqual([1, 2], sut)
+        assert [1, 2] == list(sut)
         with assert_not_reactor_called(sut):
             reactive_value.react.trigger()
 
     def test_remove(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([reactive_value])
+        sut = ReactiveMutableSequence[Reactive]([reactive_value])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut.remove(reactive_value)
-        self.assertEqual([], sut)
+        assert [] == list(sut)
         with assert_not_reactor_called(sut):
             reactive_value.react.trigger()
 
-    def test_reverse(self) -> None:
-        sut = ReactiveList([1, 2, 3])
-        with assert_scope_empty():
-            with assert_reactor_called(sut):
-                sut.reverse()
-        self.assertEqual([3, 2, 1], sut)
-
-    def test_sort(self) -> None:
-        sut = ReactiveList([3, 2, 1])
-        with assert_scope_empty():
-            with assert_reactor_called(sut):
-                sut.sort()
-        self.assertEqual([1, 2, 3], sut)
-
-    def test_sort_with_key(self) -> None:
-        sut = ReactiveList(['xc', 'yb', 'za'])
-        with assert_scope_empty():
-            with assert_reactor_called(sut):
-                sut.sort(key=lambda x: x[1])
-        self.assertEqual(['za', 'yb', 'xc'], sut)
-
-    def test_sort_with_reversed(self) -> None:
-        sut = ReactiveList([1, 2, 3])
-        with assert_scope_empty():
-            with assert_reactor_called(sut):
-                sut.sort(reverse=True)
-        self.assertEqual([3, 2, 1], sut)
-
-    def test_add(self) -> None:
-        reactive_value = _Reactive()
-        sut = ReactiveList([reactive_value])
-        other = [1, 2]
-        with assert_scope_empty():
-            with assert_not_reactor_called(sut):
-                new_sut = sut + other
-        self.assertEqual([reactive_value, 1, 2], new_sut)
-        with assert_reactor_called(new_sut):
-            reactive_value.react.trigger()
-
-    def test_contains(self) -> None:
-        sut = ReactiveList([1])
-        with assert_in_scope(sut):
-            self.assertIn(1, sut)
-            self.assertNotIn(2, sut)
-
     def test_delitem(self) -> None:
         reactive_value = _Reactive()
-        sut = ReactiveList([reactive_value])
+        sut = ReactiveMutableSequence[Reactive]([reactive_value])
         with assert_scope_empty():
             with assert_reactor_called(sut):
                 del sut[0]
-        self.assertEqual([], sut)
-        self.assertEqual([], reactive_value.react._reactors)
-
-    def test_eq(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual([1, 2], sut)
-
-    def test_getitem(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual(2, sut[1])
+        assert [] == list(sut)
+        with assert_not_reactor_called(sut):
+            reactive_value.react.trigger()
 
     def test_iadd(self) -> None:
         reactive_value1 = _Reactive()
         reactive_value2 = _Reactive()
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1, 2])
+        with assert_scope_empty():
             with assert_reactor_called(sut):
                 sut += [reactive_value1, reactive_value2]
-        self.assertEqual([1, 2, reactive_value1, reactive_value2], sut)
+        assert [1, 2, reactive_value1, reactive_value2] == list(sut)
         with assert_reactor_called(sut):
             reactive_value1.react.trigger()
         with assert_reactor_called(sut):
             reactive_value2.react.trigger()
 
-    def test_imul(self) -> None:
-        reactive_value1 = _Reactive()
-        reactive_value2 = _Reactive()
-        sut = ReactiveList([reactive_value1, reactive_value2])
-        with assert_in_scope(sut):
+    def test___setitem__with_int(self) -> None:
+        reactive_value = _Reactive()
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1])
+        with assert_scope_empty():
             with assert_reactor_called(sut):
-                sut *= 2
-        self.assertEqual([reactive_value1, reactive_value2, reactive_value1, reactive_value2], sut)
-        with assert_reactor_called(sut):
-            reactive_value1.react.trigger()
+                sut[0] = reactive_value
+        assert reactive_value == sut[0]
         with assert_reactor_called(sut):
-            reactive_value2.react.trigger()
-
-    def test_iter(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual([1, 2], list(iter(sut)))
-
-    def test_len(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual(2, len(sut))
-
-    def test_mul(self) -> None:
-        reactive_value1 = _Reactive()
-        reactive_value2 = _Reactive()
-        sut = ReactiveList([reactive_value1, reactive_value2])
-        with assert_scope_empty():
-            with assert_not_reactor_called(sut):
-                new_sut = sut * 2
-        self.assertEqual([reactive_value1, reactive_value2, reactive_value1, reactive_value2], new_sut)
-        with assert_reactor_called(new_sut):
-            reactive_value1.react.trigger()
-        with assert_reactor_called(new_sut):
-            reactive_value2.react.trigger()
-
-    def test_ne(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertNotEqual([2, 1], sut)
-
-    def test_reversed(self) -> None:
-        sut = ReactiveList([1, 2])
-        with assert_in_scope(sut):
-            self.assertEqual([2, 1], list(reversed(sut)))
-
-    def test_rmul(self) -> None:
-        reactive_value1 = _Reactive()
-        reactive_value2 = _Reactive()
-        sut = ReactiveList([reactive_value1, reactive_value2])
-        with assert_scope_empty():
-            with assert_not_reactor_called(sut):
-                new_sut = 2 * sut
-        self.assertEqual([reactive_value1, reactive_value2, reactive_value1, reactive_value2], new_sut)
-        with assert_reactor_called(new_sut):
-            reactive_value1.react.trigger()
-        with assert_reactor_called(new_sut):
-            reactive_value2.react.trigger()
+            reactive_value.react.trigger()
 
-    def test_setitem(self) -> None:
-        reactive_value = _Reactive()
-        sut = ReactiveList([1, 2])
+    def test___setitem__with_slice(self) -> None:
+        reactive_value_1 = _Reactive()
+        reactive_value_2 = _Reactive()
+        sut = ReactiveMutableSequence[Union[Reactive, int]]([1])
         with assert_scope_empty():
             with assert_reactor_called(sut):
-                sut[1] = reactive_value
-        self.assertEqual(reactive_value, sut[1])
+                sut[0:2] = reactive_value_1, reactive_value_2
+        assert [reactive_value_1, reactive_value_2] == list(sut[0:2])
         with assert_reactor_called(sut):
-            reactive_value.react.trigger()
+            reactive_value_1.react.trigger()
+        with assert_reactor_called(sut):
+            reactive_value_2.react.trigger()
+
+    def test___getitem__with_int(self) -> None:
+        sut = ReactiveMutableSequence[int]([1, 2])
+        with assert_in_scope(sut):
+            assert 2 == sut[1]
 
-    def test_sizeof(self) -> None:
-        sut = ReactiveList([1, 2])
+    def test___getitem__with_slice(self) -> None:
+        sut = ReactiveMutableSequence[int]([1, 2])
         with assert_in_scope(sut):
-            sys.getsizeof(sut)
+            assert [1, 2] == list(sut[0:2])
```

### Comparing `reactives-0.4.3/reactives/tests/test_reactor.py` & `reactives-0.5.0/reactives/tests/test_reactor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,165 +1,270 @@
 import copy
-import gc
-from unittest import TestCase
+from typing import Any, MutableSequence
 
+import pytest
 from parameterized import parameterized
 
 from reactives import Reactive
-from reactives.reactor import ReactorController, resolve_reactor, resolve_reactor_controller, ExpectedCallCount
+from reactives.reactor import ReactorController, resolve_reactor_controller, ExpectedCallCount, _ReactorChain, \
+    TriggerOrigin
 from reactives.tests import assert_reactor_called, assert_not_reactor_called, AssertCallCountReactor
 
 
 class _Reactive(Reactive):
-    def __init__(self, *args, **kwargs):
+    def __init__(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(*args, **kwargs)
         self.react = ReactorController()
 
 
-class ReactorControllerTest(TestCase):
+class OnTriggerReactorController(ReactorController):
+    def __init__(self) -> None:
+        super().__init__()
+        self.tracker: MutableSequence[bool] = []
+
+    def _on_trigger(self) -> None:
+        self.tracker.append(True)
+
+
+class NeverExternalTriggerReactorController(ReactorController):
+    def __init__(self) -> None:
+        super().__init__()
+        self.tracker: MutableSequence[bool] = []
+
+    def _on_trigger(self) -> None:
+        raise AssertionError('This reactor controller must never be triggered externally.')
+
+
+class TestReactorChain:
+    def test_trigger_without_reactors(self) -> None:
+        reactor_controller = ReactorController()
+        sut = _ReactorChain()
+        sut.trigger(reactor_controller)
+
+    def test_trigger_with_reactor(self) -> None:
+        reactor_controller = ReactorController()
+        sut = _ReactorChain()
+        with assert_reactor_called(reactor_controller):
+            sut.trigger(reactor_controller)
+
+    def test_trigger_with_origin_external(self) -> None:
+        reactor_controller_1 = OnTriggerReactorController()
+        reactor_controller_2 = OnTriggerReactorController()
+        reactor_controller_1.react(reactor_controller_2)
+        sut = _ReactorChain()
+        with assert_reactor_called(reactor_controller_1):
+            with assert_reactor_called(reactor_controller_2):
+                sut.trigger(reactor_controller_1, origin=TriggerOrigin.EXTERNAL)
+        assert [True] == reactor_controller_1.tracker
+        assert [True] == reactor_controller_2.tracker
+
+    def test_trigger_with_origin_internal(self) -> None:
+        reactor_controller_1 = NeverExternalTriggerReactorController()
+        reactor_controller_2 = OnTriggerReactorController()
+        reactor_controller_1.react(reactor_controller_2)
+        sut = _ReactorChain()
+        with assert_reactor_called(reactor_controller_1):
+            with assert_reactor_called(reactor_controller_2):
+                sut.trigger(reactor_controller_1, origin=TriggerOrigin.INTERNAL)
+        assert [] == reactor_controller_1.tracker
+        assert [True] == reactor_controller_2.tracker
+
+    def test_trigger_with_diamond_reactors(self) -> None:
+        order_tracker = []
+        r_a = _Reactive()
+        r_b = _Reactive()
+        r_ba = _Reactive()
+        r_c = _Reactive()
+        r_ca = _Reactive()
+        r_d = _Reactive()
+
+        r_a.react(lambda: order_tracker.append('a'))
+        r_a.react(r_b)
+        r_a.react(r_c)
+        r_b.react(lambda: order_tracker.append('b'))
+        r_b.react(r_ba)
+        r_ba.react(lambda: order_tracker.append('ba'))
+        r_ba.react(r_d)
+        r_c.react(lambda: order_tracker.append('c'))
+        r_c.react(r_ca)
+        r_ca.react(lambda: order_tracker.append('ca'))
+        r_ca.react(r_d)
+        r_d.react(lambda: order_tracker.append('d'))
+
+        sut = _ReactorChain()
+        sut.trigger(r_a.react)
+
+        # The reactors are laid out as follows, with all relationships being predefined through reactors.
+        #
+        #     r_a
+        #     / \
+        #  r_b   r_c
+        #   |     |
+        # r_ba   r_ca
+        #    \   /
+        #     r_d
+        assert ['a', 'b', 'c', 'ba', 'ca', 'd'] == order_tracker
+
+    def test_trigger_with_diamond_triggers(self) -> None:
+        order_tracker = []
+        r_a = _Reactive()
+        r_b = _Reactive()
+        r_ba = _Reactive()
+        r_c = _Reactive()
+        r_ca = _Reactive()
+        r_d = _Reactive()
+
+        def f_a() -> None:
+            order_tracker.append('a')
+            r_b.react.trigger()
+            r_c.react.trigger()
+        r_a.react(f_a)
+
+        def f_b() -> None:
+            order_tracker.append('b')
+            r_ba.react.trigger()
+        r_b.react(f_b)
+
+        def f_ba() -> None:
+            order_tracker.append('ba')
+            r_d.react.trigger()
+        r_ba.react(f_ba)
+
+        def f_c() -> None:
+            order_tracker.append('c')
+            r_ca.react.trigger()
+        r_c.react(f_c)
+
+        def f_ca() -> None:
+            order_tracker.append('ca')
+            r_d.react.trigger()
+        r_ca.react(f_ca)
+
+        def f_d() -> None:
+            order_tracker.append('d')
+        r_d.react(f_d)
+
+        sut = _ReactorChain()
+        sut.trigger(r_a.react)
+
+        # The reactors are laid out as follows, with all relationships being defined through triggers from one reactor
+        # to another reactive.
+        #
+        #     f_a
+        #     / \
+        #  f_b   f_c
+        #   |     |
+        # f_ba   f_ca
+        #    \   /
+        #     f_d
+        #
+        # 'd' appears in the resolved chain twice. Due to the non-declarative nature of triggers, the 'ba' trigger of
+        # 'd' is completed by the time 'ca' is triggered and can trigger 'd' again.
+        assert ['a', 'b', 'ba', 'd', 'c', 'ca', 'd'] == order_tracker
+
+
+class TestReactorController:
     def test___copy__(self) -> None:
         sut = ReactorController()
         with assert_reactor_called(sut):
             copied_sut = copy.copy(sut)
             with assert_not_reactor_called(sut):
                 with assert_reactor_called(copied_sut):
                     copied_sut.trigger()
 
-    def test_react_without_reactors(self) -> None:
+    def test_trigger_with_on_trigger(self) -> None:
+        sut = OnTriggerReactorController()
+        sut.trigger()
+        assert [True] == sut.tracker
+
+    def test_trigger_with_on_trigger_with_reactor(self) -> None:
+        sut = OnTriggerReactorController()
+        sut.react(lambda: sut.tracker.append(False))
+        sut.trigger()
+        assert [True, False] == sut.tracker
+
+    def test_trigger_without_reactors(self) -> None:
         sut = ReactorController()
         sut.trigger()
 
     def test_react_with_reactor(self) -> None:
         sut = ReactorController()
-        with assert_reactor_called() as reactor:
-            sut.react(reactor)
-            sut.trigger()
-
-    def test_react_with_diamond_reactors(self) -> None:
-        sut = ReactorController()
-        with assert_reactor_called() as final_reactor:
-            intermediate_reactive_1 = _Reactive()
-            intermediate_reactive_2 = _Reactive()
-            intermediate_reactive_1.react(final_reactor)
-            intermediate_reactive_2.react(final_reactor)
-            sut.react(intermediate_reactive_1)
-            sut.react(intermediate_reactive_2)
-            sut.trigger()
-
-    def test_react_with_intermediate_diamond_reactors(self) -> None:
-        order_tracker = []
-        r_a = _Reactive()
-        r_a.react(lambda: order_tracker.append('r_a'))
-        r_b = _Reactive()
-        r_b.react(lambda: order_tracker.append('r_b'))
-        r_c = _Reactive()
-        r_c.react(lambda: order_tracker.append('r_c'))
-        r_d = _Reactive()
-        r_d.react(lambda: order_tracker.append('r_d'))
-        r_da = _Reactive()
-        r_da.react(lambda: order_tracker.append('r_da'))
-        r_e = _Reactive()
-        r_e.react(lambda: order_tracker.append('r_e'))
-
-        r_a.react(r_b)
-        r_b.react(r_c)
-        r_b.react(r_d)
+        reactor = AssertCallCountReactor(sut)
+        sut.react(reactor)
+        sut.trigger()
+        reactor.assert_call_count()
 
-        # This is the intermediate trigger we are asserting is consolidated into the reactor chain.
-        def f_ca():
-            order_tracker.append('f_ca')
-            r_e.react.trigger()
-        r_c.react(f_ca)
-        r_d.react(r_da)
-        r_da.react(r_e)
-
-        r_a.react.trigger()
-        self.assertEqual(['r_a', 'r_b', 'r_c', 'f_ca', 'r_d', 'r_da', 'r_e'], order_tracker)
-
-    def test_react_using_shortcut_with_reactor(self) -> None:
-        sut = ReactorController()
-        with assert_reactor_called() as reactor:
-            sut(reactor)
-            sut.trigger()
+    def test___call___with_reactor(self) -> None:
+        sut = ReactorController()
+        reactor = AssertCallCountReactor(sut)
+        sut(reactor)
+        sut.trigger()
+        reactor.assert_call_count()
 
     def test_shutdown(self) -> None:
         sut = ReactorController()
-        with assert_not_reactor_called() as reactor_1:
-            with assert_not_reactor_called() as reactor_2:
-                sut.react(reactor_1, reactor_2)
-                sut.shutdown()
-                sut.trigger()
+        reactor_not_called_one = AssertCallCountReactor(sut, 0)
+        reactor_not_called_two = AssertCallCountReactor(sut, 0)
+        sut.react(reactor_not_called_one, reactor_not_called_two)
+        sut.shutdown()
+        sut.trigger()
+        reactor_not_called_one.assert_call_count()
+        reactor_not_called_two.assert_call_count()
 
     def test_shutdown_with_specified_reactors(self) -> None:
         sut = ReactorController()
-        with assert_reactor_called() as reactor_called:
-            with assert_not_reactor_called() as reactor_not_called:
-                sut.react(reactor_called, reactor_not_called)
-                sut.shutdown(reactor_not_called)
-                sut.trigger()
+        reactor_called = AssertCallCountReactor(sut)
+        reactor_not_called = AssertCallCountReactor(sut, 0)
+        sut.react(reactor_called, reactor_not_called)
+        sut.shutdown(reactor_not_called)
+        sut.trigger()
+        reactor_called.assert_call_count()
+        reactor_not_called.assert_call_count()
+
+    def test_react_weakref_with_method(self) -> None:
+        sut = ReactorController()
+
+        class _Raise:
+            def _raise(self) -> None:
+                AssertCallCountReactor(sut, 0)()
+        _raise = _Raise()
+        sut.react_weakref(_raise._raise)
+        del _raise
+        sut.trigger()
 
     def test_react_weakref(self) -> None:
         sut = ReactorController()
-        reactor = AssertCallCountReactor(0)
+        reactor = AssertCallCountReactor(sut, 0)
         sut.react_weakref(reactor)
         del reactor
-        gc.collect()
         sut.trigger()
 
-    def test_suspend(self) -> None:
-        sut = ReactorController()
-        with assert_not_reactor_called() as reactor:
-            sut.react_weakref(reactor)
-            with ReactorController.suspend():
-                sut.trigger()
-
-
-class ResolveReactorTest(TestCase):
-    def test_with_reactor(self) -> None:
-        def _reactor() -> None:
-            pass
-        resolvable = _reactor
-        self.assertSequenceEqual((resolvable,), tuple(resolve_reactor(resolvable)))
-
-    def test_with_reactor_controller(self) -> None:
-        def _reactor() -> None:
-            pass
-        resolvable = ReactorController()
-        resolvable.react(_reactor)
-        self.assertSequenceEqual((_reactor,), tuple(resolve_reactor(resolvable)))
-
-    def test_with_reactive(self) -> None:
-        def _reactor() -> None:
-            pass
 
-        class _Reactive(Reactive):
-            def __init__(self):
-                self.react = ReactorController()
-        resolvable = _Reactive()
-        resolvable.react(_reactor)
-        self.assertSequenceEqual((_reactor,), tuple(resolve_reactor(resolvable)))
-
-
-class ResolveReactorControllerTest(TestCase):
+class TestResolveReactorController:
     def test_with_reactor_controller(self) -> None:
         reactor_controller = ReactorController()
         resolvable = reactor_controller
-        self.assertEqual(reactor_controller, resolve_reactor_controller(resolvable))
+        assert reactor_controller == resolve_reactor_controller(resolvable)
 
     def test_with_reactive(self) -> None:
         reactor_controller = ReactorController()
 
         class _Reactive(Reactive):
-            def __init__(self):
+            def __init__(self) -> None:
+                super().__init__()
                 self.react = reactor_controller
         resolvable = _Reactive()
-        self.assertEqual(reactor_controller, resolve_reactor_controller(resolvable))
+        assert reactor_controller == resolve_reactor_controller(resolvable)
 
 
-class AssertCallCountReactorTest(TestCase):
+class TestAssertCallCountReactor:
     @parameterized.expand([
         (0, 0),
         (1, 1),
         (2, 2),
         ((1, 3), 1),
         ((1, 3), 2),
         ((1, 3), 3),
@@ -173,15 +278,16 @@
         (1, 2),
         (2, 1),
         (2, 3),
         ((1, 3), 0),
         ((1, 3), 4),
     ])
     def test_assert_call_count_should_raise_error(self, expected_call_count: ExpectedCallCount, actual_call_count: int) -> None:
-        with self.assertRaises(AssertionError):
+        with pytest.raises(AssertionError):
             self._assert_call_count(expected_call_count, actual_call_count)
 
     def _assert_call_count(self, expected_call_count: ExpectedCallCount, actual_call_count: int) -> None:
-        sut = AssertCallCountReactor(expected_call_count)
+        reactor_controller = ReactorController()
+        sut = AssertCallCountReactor(reactor_controller, expected_call_count)
         for _ in range(0, actual_call_count):
             sut()
         sut.assert_call_count()
```

### Comparing `reactives-0.4.3/reactives/tests/test_scope.py` & `reactives-0.5.0/reactives/tests/test_scope.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from unittest import TestCase
-
 from reactives import scope, Reactive
 from reactives.reactor import ReactorController
 
 
 class _NotReactive:
     pass
 
 
 class _NotReactiveWithAttribute:
-    def __init__(self):
+    def __init__(self) -> None:
         self.react = None
 
 
 class _Reactive(Reactive):
-    def __init__(self):
+    def __init__(self) -> None:
+        super().__init__()
         self.react = ReactorController()
 
 
-class CollectTest(TestCase):
+class TestCollect:
     def test_without_dependencies(self) -> None:
         reactive = _Reactive()
         with scope.collect(reactive):
             pass
-        self.assertEqual([], reactive.react._dependencies)
+        assert [] == reactive.react._dependencies
 
     def test_with_dependency(self) -> None:
         reactive = _Reactive()
         dependency = _Reactive()
         with scope.collect(reactive):
             scope.register(dependency)
-        self.assertEqual([dependency], reactive.react._dependencies)
+        assert dependency.react in reactive.react._dependencies
```

### Comparing `reactives-0.4.3/reactives.egg-info/PKG-INFO` & `reactives-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: reactives
-Version: 0.4.3
-Summary: A declarative reactive programming framework.
-Home-page: https://github.com/bartfeenstra/reactives
-Author: Bart Feenstra & contributors
-Author-email: bart@mynameisbart.com
-License: GPLv3
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~= 3.7
-Description-Content-Type: text/markdown
-Provides-Extra: development
-License-File: LICENSE.txt
-
 
 # Reactives
 
 ![Test status](https://github.com/bartfeenstra/reactives/workflows/Test/badge.svg) [![Code coverage](https://codecov.io/gh/bartfeenstra/reactives/branch/main/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/reactives) [![PyPI releases](https://badge.fury.io/py/reactives.svg)](https://pypi.org/project/reactives/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/reactives.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/reactives/) [![Recent downloads](https://img.shields.io/pypi/dm/reactives.svg)](https://pypi.org/project/reactives/) 
 
 **Reactives** lets you write reactive code easily by making any of your objects and functions *reactive*. A reactive
 can be *triggered* (`reactive.react.trigger()`), causing all its *reactors* to be called. A *reactor* is any callable
@@ -30,166 +9,140 @@
 its reactors and its reactors' reactors are resolved, and each is called once in order.
 
 **Reactives** uses a push-pull approach, meaning change notifications are pushed (reactors are called automatically and
 won't have to pull for changes), but if a reactor needs to know what exactly changed, it must pull this information
 itself.
 
 ## Usage
-For any type to be reactive, it must extend `reactives.factory.Reactive` and set a `reactives.ReactorController`
-instance in its `__init__()` method. For any of the types supported by default, you only have to decorate your type or
-value with `@reactives.reactive`. Additionally, some classes are provided that are reactive and can be instantiated or
-inherited from directly.
+For any type to be reactive, it must extend `reactives.Reactive` and expose a `reactives.reactor.ReactorController`
+instance through its `react` instance attribute.
+
+**Reactives** provides the reactive framework, the tools to make your own types reactive, and several fully reactive
+types out of the box, batteries included!
 
 ### Custom classes
 Decorate a class to make its individual instances reactive:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     pass
 
 apple = Apple()
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 ### Functions and methods 
 Decorate a function:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive
+@reactive_function
 def apple():
     pass
 
 apple.react(lambda: print('The apple got triggered!'))
 apple.react.trigger()
 # >>> "The apple got triggered!"
 ```
 
 Decorate a method on a **reactive class**:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.method import reactive_method
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
+    @reactive_method
     def apple(self):
         pass
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 Reactive methods must be accessed through their instance, because `Apple.apple` would yield the class method.
 
 Both functions and methods can be called automatically when they're triggered. This lets them set up something once, and
 update that thing when they're triggered:
 ```python
-from reactives import reactive
+from reactives.function import reactive_function
 
-@reactive(on_trigger_call=True)
+@reactive_function(on_trigger_call=True)
 def warm_caches():
     """
     Warm the application's caches. When triggered (because the cached data has changed), re-warm the caches.
     """
     pass
 ```
 
 ### Properties
 Decorate a property:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
-    @reactive
+class Apple(ReactiveInstance):
     @property
+    @reactive_property
     def apple(self) -> str:
         return 'I got you something!'
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.react['apple'].react.trigger()
 # >>> "The apple got triggered!"
 ```
 
-If a property *deleter* is present, it will be called automatically when the property is triggered:
+If a property *deleter* is present, it may be called automatically when the property is triggered:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._cached_something = None
 
-    @reactive
     @property
+    @reactive_property(on_trigger_delete=True)
     def apple(self) -> str:
         if self._cached_something is None:
             self._cached_something = 'I got you something!'
         return self._cached_something
 
     @apple.deleter
     def apple(self)  -> None:
         self._cached_something = 'I got you nothing!'
 
 apple = Apple()
 print(apple.apple)
 # >>> "I got you something!"
-apple.react['apple'].react().trigger()
+apple.react['apple'].react.trigger()
 print(apple.apple)
 # >>> "I got you nothing!"
 ```
 
-If you do not want automatic deletion, configure the property's `@reactive` decorator as such:
-```python
-from reactives import reactive
-
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(on_trigger_delete=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            self._cached_something = 'I got you something!'
-        return self._cached_something
-
-    @apple.deleter
-    def apple(self)  -> None:
-        self._cached_something = 'I got you nothing!'
-
-apple = Apple()
-print(apple.apple)
-# >>> "I got you something!"
-apple.react['apple'].react().trigger()
-print(apple.apple)
-# >>> "I got you something!"
-```
-
 Property *setters* work exactly like with any other `property`:
 ```python
-from reactives import reactive
+from reactives.instance import ReactiveInstance
+from reactives.instance.property import reactive_property
 
-@reactive
-class Apple:
+class Apple(ReactiveInstance):
     def __init__(self):
+        super().__init__()
         self._something = 'I got you something!'
-        
-    @reactive
+
     @property
+    @reactive_property
     def apple(self) -> str:
         return self._something
-    
+
     @apple.setter
     def apple(self, something: str):
         self._something = something
 
 apple = Apple()
 apple.react['apple'].react(lambda: print('The apple got triggered!'))
 apple.apple = 'I got you something else!'
@@ -197,71 +150,51 @@
 ```
 
 Values set through a property may themselves be reactive too. If they are, the property and the value are autowired, 
 which means that the property becomes a reactor to the newly added value. As soon as the value is triggered,
 so is the property. Therefore, if you want to react to any change to any of the values a property might have, all you
 need to do is add your reactor to the property.
 
-*Getters* that perform conditional logic, such as for cached properties, can take over reactive scope dependency
-collection for more fine-grained reactivity control:
+### Sequences
+`reactives.collections.ReactiveSequence` and `reactives.collections.ReactiveMutableSequence` are reactive versions of 
+Python's built-in `Sequence` and `MutableSequence`, which are drop-in replacements for `list`.
 ```python
-from reactives import reactive, scope
+from reactives.collections import ReactiveMutableSequence
 
-@reactive
-class Apple:
-    def __init__(self):
-        self._cached_something = None
-
-    @reactive(auto_collect_scope=False)
-    @property
-    def apple(self) -> str:
-        if self._cached_something is None:
-            with scope.collect(self.react['apple']):
-                self._cached_something = build_something()
-        return self._cached_something
-
-def build_something():
-    pass
-```
-
-### Lists
-`ReactiveList` is a reactive version of Python's built-in `list`. You can use it in exactly the same way as `list`:
-```python
-from reactives import ReactiveList
-
-fruits = ReactiveList(['apple', 'banana'])
+fruits = ReactiveMutableSequence(['apple', 'banana'])
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits.append('orange')
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveList` may themselves be reactive too. If they are, the list and the value are autowired, 
-which means that the list becomes a reactor to the newly added value. As soon as the value is triggered,
-so is the list. Therefore, if you want to react to any change to any of the values in a `ReactiveList`, all you
-need to do is add your reactor to the list.
-
-### Dictionaries
-`ReactiveDict` is a reactive version of Python's built-in `dict`. You can use it in exactly the same way as `dict`:
+Values added to a `ReactiveSequence` or `ReactiveMutableSequence` may themselves be reactive too. If they are, the 
+sequence and the value are autowired, which means that the sequence becomes a reactor to the newly added value. As soon 
+as the value is triggered, so is the sequence. Therefore, if you want to react to any change to any of the values in a
+`ReactiveSequence` or `ReactiveMutableSequence`, all you need to do is add your reactor to the sequence.
+
+### Mappings
+`reactives.collections.ReactiveMapping` and `reactives.collections.ReactiveMutableMapping` are reactive versions of 
+Python's built-in `Mapping` and `MutableMapping`, which are drop-in replacements for `dict`.
 ```python
-from reactives import ReactiveDict
+from reactives.collections import ReactiveMutableMapping
 
-fruits = ReactiveDict(apple=5, banana=2)
+fruits = ReactiveMutableMapping(apple=5, banana=2)
 fruits.react(lambda: print('Look at all these delicious fruits!'))
 fruits['orange'] = 4
 # >>> "Look at all these delicious fruits!"
 ```
 
-Values added to a `ReactiveDict` may themselves be reactive too. If they are, the dictionary and the value are
-autowired, which means that the dictionary becomes a reactor to the newly added value. As soon as the value is
-triggered, so is the dictionary. Therefore, if you want to react to any change to any of the values in a `ReactiveDict`, 
-all you  need to do is add your reactor to the dictionary.
+Values added to a `ReactiveMapping` or `ReactiveMutableMapping` may themselves be reactive too. If they are, the 
+mapping and the value are autowired, which means that the mapping becomes a reactor to the newly added value. As soon as
+the value is triggered, so is the mapping. Therefore, if you want to react to any change to any of the values in a 
+`ReactiveMapping` or `ReactiveMutableMapping`, all you  need to do is add your reactor to the mapping.
 
 ### Autowiring
-We've seen how [properties](#Properties), [lists](#Lists), and [dictionaries](#Dictionaries) autowire themselves to
-their values. This is possible because properties, lists, and dictionaries know exactly which values move in and out of
+We've seen how [properties](#Properties), [sequences](#Sequences), and [mappings](#Mappings) autowire themselves to
+their values. This is possible because properties, sequences, and mappings know exactly which values move in and out of
 them. In other cases, we use *scope*. Any reactive can start a scope with `reactives.scope.collect()` and collect all
 reactives that are called or used during that scope window, and autowire itself to them. Conversely, any reactive can
 register itself with the current scope (if there is one) with `reactives.scope.register*()`, and allow reactives
 depending on it to autowire themselves. In fact, this is what properties do internally.
 
 Autowiring means that as a developer, you won't need to worry about connecting the parts of your application most of the
 time.
@@ -290,9 +223,7 @@
 [submit improvements](https://github.com/bartfeenstra/reactives/pulls).
 
 ## Copyright & license
 Reactives is copyright [Bart Feenstra](https://twitter.com/BartFeenstra/) and contributors, and released under the
 [GNU General Public License, Version 3](./LICENSE.txt). In short, that means **you are free to use Reactives**, but **if you
 distribute Reactives yourself, you must do so under the exact same license**, provide that license, and make your source
 code available. 
-
-
```

### Comparing `reactives-0.4.3/reactives.egg-info/SOURCES.txt` & `reactives-0.5.0/reactives.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 LICENSE.txt
 README.md
 VERSION
 setup.py
 reactives/__init__.py
+reactives/_callable.py
+reactives/_decorator.py
 reactives/collections.py
+reactives/function.py
 reactives/py.typed
 reactives/reactor.py
 reactives/scope.py
 reactives.egg-info/PKG-INFO
 reactives.egg-info/SOURCES.txt
 reactives.egg-info/dependency_links.txt
 reactives.egg-info/requires.txt
 reactives.egg-info/top_level.txt
-reactives/factory/__init__.py
-reactives/factory/function.py
-reactives/factory/property.py
-reactives/factory/type.py
+reactives/instance/__init__.py
+reactives/instance/method.py
+reactives/instance/property.py
 reactives/tests/__init__.py
+reactives/tests/test__callable.py
 reactives/tests/test_collections.py
+reactives/tests/test_function.py
 reactives/tests/test_reactor.py
 reactives/tests/test_scope.py
-reactives/tests/factory/__init__.py
-reactives/tests/factory/test___init__.py
-reactives/tests/factory/test_function.py
-reactives/tests/factory/test_property.py
-reactives/tests/factory/test_type.py
+reactives/tests/instance/__init__.py
+reactives/tests/instance/test___init__.py
+reactives/tests/instance/test_method.py
+reactives/tests/instance/test_property.py
```

### Comparing `reactives-0.4.3/setup.py` & `reactives-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,39 @@
     'license': 'GPLv3',
     'author': 'Bart Feenstra & contributors',
     'author_email': 'bart@mynameisbart.com',
     'url': 'https://github.com/bartfeenstra/reactives',
     'classifiers': [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
+        'Typing :: Typed',
     ],
-    'python_requires': '~= 3.7',
+    'python_requires': '~= 3.8',
     'install_requires': [
-        'graphlib-backport ~= 1.0; python_version < "3.9"',
+        'graphlib-backport ~= 1.0.3; python_version < "3.9"',
+        'typing_extensions ~= 4.4.0; python_version < "3.11"',
     ],
     'extras_require': {
         'development': [
             'autopep8 ~= 1.6.0',
             'codecov ~= 2.1.12',
             'coverage ~= 6.3.2',
             'dill ~= 0.3.4',
-            'flake8 ~= 4.0.1',
-            'mypy ~= 0.950',
-            'nose2 ~= 0.11.0',
+            'flake8 ~= 6.0.0',
+            'mypy ~= 1.2.0',
             'parameterized ~= 0.8.1',
+            'pytest ~= 7.2.0',
+            'pytest-cov ~= 4.0.0',
             'setuptools ~= 62.1.0',
             'twine ~= 4.0',
-            'typing_extensions ~= 4.2.0; python_version < "3.10"',
             'wheel ~= 0.37.1',
         ],
     },
     'packages': find_packages(),
     'data_files': [
         ('', [
             'LICENSE.txt',
```


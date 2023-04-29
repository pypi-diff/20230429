# Comparing `tmp/lightbulb_ext_hecate-0.1.5.tar.gz` & `tmp/lightbulb_ext_hecate-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightbulb_ext_hecate-0.1.5.tar", max compression
+gzip compressed data, was "lightbulb_ext_hecate-0.1.6.tar", max compression
```

## Comparing `lightbulb_ext_hecate-0.1.5.tar` & `lightbulb_ext_hecate-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1084 2023-02-08 23:33:47.412225 lightbulb_ext_hecate-0.1.5/LICENSE
--rw-r--r--   0        0        0      471 2023-02-16 18:21:43.843406 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/__init__.py
--rw-r--r--   0        0        0      855 2023-02-16 18:56:12.788517 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/__main__.py
--rw-r--r--   0        0        0     1057 2023-02-14 16:58:08.667242 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/errors.py
--rw-r--r--   0        0        0     1828 2023-02-16 20:53:04.597535 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/params.py
--rw-r--r--   0        0        0     9564 2023-02-16 23:53:10.160459 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/plugin.py
--rw-r--r--   0        0        0     1432 2023-02-17 00:09:13.925340 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/properties.py
--rw-r--r--   0        0        0      671 2023-02-17 00:12:11.861168 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/__modify__.py
--rw-r--r--   0        0        0      986 2023-02-16 20:55:08.927271 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/slash-commands/ping.py
--rw-r--r--   0        0        0      681 2023-02-16 23:26:38.679786 lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/slash-commands/pong_count.py
--rw-r--r--   0        0        0      515 2023-02-16 18:20:52.267394 lightbulb_ext_hecate-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1022 2023-02-16 20:36:11.359710 lightbulb_ext_hecate-0.1.5/README.md
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 lightbulb_ext_hecate-0.1.5/setup.py
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 lightbulb_ext_hecate-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5763 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/README.md
+-rw-r--r--   0        0        0      451 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/__main__.py
+-rw-r--r--   0        0        0     1020 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/errors.py
+-rw-r--r--   0        0        0     1776 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/params.py
+-rw-r--r--   0        0        0     9341 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/plugin.py
+-rw-r--r--   0        0        0     1452 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/properties.py
+-rw-r--r--   0        0        0      651 2023-04-29 17:31:56.554720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/__modify__.py
+-rw-r--r--   0        0        0      354 2023-04-29 17:31:56.558720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/events/GuildMessageCreateEvent.py
+-rw-r--r--   0        0        0      450 2023-04-29 17:31:56.558720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/events/_GuildMessageDeleteEvent.py
+-rw-r--r--   0        0        0      959 2023-04-29 17:31:56.558720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/slash-commands/ping.py
+-rw-r--r--   0        0        0      663 2023-04-29 17:31:56.558720 lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/slash-commands/pong_count.py
+-rw-r--r--   0        0        0      496 2023-04-29 17:31:56.558720 lightbulb_ext_hecate-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6463 1970-01-01 00:00:00.000000 lightbulb_ext_hecate-0.1.6/PKG-INFO
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/__main__.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/__main__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import argparse
-import os.path as osp
-from distutils.dir_util import copy_tree
-
-# argparsing stuff
-parser = argparse.ArgumentParser(description='Acts upon existing lightbulb extension modules.', prog='lightbulb.ext.hecate')
-parser.add_argument('--template', metavar='EXT_PATH', dest='ext_path',
-                help='generates template files for the extension file at EXT_PATH')
-args = parser.parse_args()
-
-# Check that the path is a python file
-if not osp.exists(args.ext_path) or not args.ext_path.endswith('.py'):
-    raise FileNotFoundError("The path provided is not a python file")
-
-# Copy the contents of the 'template' folder into the dir of the provided file
-copy_tree(osp.join(osp.dirname(__file__), 'template'), osp.dirname(args.ext_path))
-print(f"Generated template for extension '{osp.basename(args.ext_path)}' successfully")
+import argparse
+import os.path as osp
+from distutils.dir_util import copy_tree
+
+# argparsing stuff
+parser = argparse.ArgumentParser(description='Acts upon existing lightbulb extension modules.', prog='lightbulb.ext.hecate')
+parser.add_argument('--template', metavar='EXT_PATH', dest='ext_path',
+                help='generates template files for the extension file at EXT_PATH')
+args = parser.parse_args()
+
+# Check that the path is a python file
+if not osp.exists(args.ext_path) or not args.ext_path.endswith('.py'):
+    raise FileNotFoundError("The path provided is not a python file")
+
+# Copy the contents of the 'template' folder into the dir of the provided file
+copy_tree(osp.join(osp.dirname(__file__), 'template'), osp.dirname(args.ext_path))
+print(f"Generated template for extension '{osp.basename(args.ext_path)}' successfully")
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/errors.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/errors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from lightbulb import LightbulbError
-
-__all__ = [
-    "HecateError",
-    "MissingParamsError",
-    "MissingMethodError",
-    "MissingHikariEventError"
-]
-
-class HecateError(LightbulbError):
-    """
-    Base hecate exception class. All errors raised by hecate will be a subclass
-    of this exception.
-    """
-
-class MissingParamsError(HecateError):
-    '''
-    Exception raised when a command module accessed by a hecate `Plugin` does not
-    contain a `params` attribute or the required params attributes in separate.
-    '''
-
-class MissingMethodError(HecateError):
-    '''
-    Exception raised when a module accessed by a hecate `Plugin` does not declare a
-    `command` or `event` method.
-    '''
-
-class MissingHikariEventError(HecateError):
-    '''
-    Exception raised when an event module accessed by a hecate `Plugin` has a name
-    that doesn't match any hikari events.
-    '''
-   
-class PropertyBuildError(HecateError):
-    '''
-    Exception raised when a property object is created with a truthy value.
-    '''
+from lightbulb import LightbulbError
+
+__all__ = [
+    "HecateError",
+    "MissingParamsError",
+    "MissingMethodError",
+    "MissingHikariEventError"
+]
+
+class HecateError(LightbulbError):
+    """
+    Base hecate exception class. All errors raised by hecate will be a subclass
+    of this exception.
+    """
+
+class MissingParamsError(HecateError):
+    '''
+    Exception raised when a command module accessed by a hecate `Plugin` does not
+    contain a `params` attribute or the required params attributes in separate.
+    '''
+
+class MissingMethodError(HecateError):
+    '''
+    Exception raised when a module accessed by a hecate `Plugin` does not declare a
+    `command` or `event` method.
+    '''
+
+class MissingHikariEventError(HecateError):
+    '''
+    Exception raised when an event module accessed by a hecate `Plugin` has a name
+    that doesn't match any hikari events.
+    '''
+   
+class PropertyBuildError(HecateError):
+    '''
+    Exception raised when a property object is created with a truthy value.
+    '''
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/params.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/params.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import hikari
-import lightbulb
-
-__all__ = [
-    "Option",
-    "Params"
-]
-
-class Option():
-    '''
-    Class that serves as an option for a given command. Should always be instantiated
-    as an element of an `options` attribute or passed into a `Params` class.
-
-    Args:
-        name (`str`): The name of the option, often in python_case.
-        description (`str`): The description of the option.
-        var_type (`hikari.OptionType`): The type of variable the option takes.
-    '''
-    def __init__(
-        self, 
-        name: str, 
-        description: str, 
-        var_type: hikari.OptionType
-    ) -> None:
-        self.name = name
-        self.description = description
-        self.var_type = var_type
-
-    def process_module(self, mod):
-        mod.command = lightbulb.option(self.name, self.description, self.var_type)(mod.command)
-
-class Params():
-    '''
-    Class that serves as the parameters for a given command. Should always be assigned to a 
-    `params` attribute in the command file. All the argument names of the `Params` class
-    constructor can also be used to define attributes, which will achieve the same effect.
-
-    Args:
-        description (`str`): The description of the command.
-        options (`list[hecate.Option]`): All the options of the command. `[]` by default.
-        name (`str`): The name of the command. `""` by default, which grabs the name from
-        the file.
-    '''
-    def __init__(self, description: str, options=[], name="") -> None:
-        self.description = description
-        self.options = options
-        self.name = name
-
-    def process_module(self, mod):
-        mod.command = lightbulb.command(self.name, self.description)(mod.command)
-        for opt in self.options:
-            opt.process_module(mod)
+import hikari
+import lightbulb
+
+__all__ = [
+    "Option",
+    "Params"
+]
+
+class Option():
+    '''
+    Class that serves as an option for a given command. Should always be instantiated
+    as an element of an `options` attribute or passed into a `Params` class.
+
+    Args:
+        name (`str`): The name of the option, often in python_case.
+        description (`str`): The description of the option.
+        var_type (`hikari.OptionType`): The type of variable the option takes.
+    '''
+    def __init__(
+        self, 
+        name: str, 
+        description: str, 
+        var_type: hikari.OptionType
+    ) -> None:
+        self.name = name
+        self.description = description
+        self.var_type = var_type
+
+    def process_module(self, mod):
+        mod.command = lightbulb.option(self.name, self.description, self.var_type)(mod.command)
+
+class Params():
+    '''
+    Class that serves as the parameters for a given command. Should always be assigned to a 
+    `params` attribute in the command file. All the argument names of the `Params` class
+    constructor can also be used to define attributes, which will achieve the same effect.
+
+    Args:
+        description (`str`): The description of the command.
+        options (`list[hecate.Option]`): All the options of the command. `[]` by default.
+        name (`str`): The name of the command. `""` by default, which grabs the name from
+        the file.
+    '''
+    def __init__(self, description: str, options=[], name="") -> None:
+        self.description = description
+        self.options = options
+        self.name = name
+
+    def process_module(self, mod):
+        mod.command = lightbulb.command(self.name, self.description)(mod.command)
+        for opt in self.options:
+            opt.process_module(mod)
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/properties.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/properties.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from .errors import PropertyBuildError
-
-__all__ = [
-    "Properties"
-]
-
-class Properties():
-    '''
-    Class for defining shared attributes between commands and events.
-    '''
-    def __init__(self, **kwargs) -> None:
-        # for key in kwargs:
-        #     if bool(kwargs[key]):
-        #         raise PropertyBuildError(f"Property '{key}' must be initialized with an empty value.")
-        self.__property_request = kwargs
-
-    def __contains__(self, __o: object) -> bool:
-        return __o in self.__property_request
-
-    def insert(self, ext_properties: dict):
-        for key in self.__property_request:
-            if not key in ext_properties:
-                ext_properties[key] = self.__property_request[key]
-            if bool(self.__property_request[key]):
-                if bool(ext_properties[key]):
-                    raise PropertyBuildError(f"Conflicting assignment of truthy values to property '{key}' ({ext_properties[key]} and {self.__property_request[key]})")
-                else:
-                    ext_properties[key] = self.__property_request[key]
-
-    def update(self, ext_properties: dict):
-        for key in self.__property_request:
-            def getter(self):
-                return ext_properties[key]
-            def setter(self, val):
-                ext_properties[key] = val
+from .errors import PropertyBuildError
+
+__all__ = [
+    "Properties"
+]
+
+class Properties():
+    '''
+    Class for defining shared attributes between commands and events.
+
+    Args:
+        **kwargs (`dict`): A key-value pair related to a shared extension attribute.
+        It will be resolved upon instantiating the associated extension.
+    '''
+    def __init__(self, **kwargs) -> None:
+        self.__property_request = kwargs
+
+    def __contains__(self, __o: object) -> bool:
+        return __o in self.__property_request
+
+    def insert(self, ext_properties: dict):
+        for key in self.__property_request:
+            if not key in ext_properties:
+                ext_properties[key] = self.__property_request[key]
+            if bool(self.__property_request[key]):
+                if bool(ext_properties[key]) and ext_properties[key] != self.__property_request[key]:
+                    raise PropertyBuildError(f"Conflicting assignment of truthy values to property '{key}' ({ext_properties[key]} and {self.__property_request[key]})")
+                else:
+                    ext_properties[key] = self.__property_request[key]
+
+    def update(self, ext_properties: dict):
+        for key in self.__property_request:
+            def getter(self):
+                return ext_properties[key]
+            def setter(self, val):
+                ext_properties[key] = val
             setattr(self.__class__, key, property(fget=getter,fset=setter))
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/__modify__.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/__modify__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from lightbulb.ext.hecate import CommandContext, EventContext
-from lightbulb import Context
-from hikari import Event
-
-# Methods to be uncommented if need be
-
-# Handles event errors
-# async def on_event_error(e_ctx: EventContext, e: Event):
-#     pass
-
-# Handles command errors
-async def on_command_error(com_ctx: CommandContext, ctx: Context):
-    await ctx.respond(f"` > Command '{com_ctx.params.name}' threw an error :( `")
-
-# Called before a command is ran
-# async def on_command_enter(com_ctx: CommandContext, ctx: Context):
-#     pass
-
-# Called after a command is ran
-# async def on_command_exit(com_ctx: CommandContext, ctx: Context):
+from lightbulb.ext.hecate import CommandContext, EventContext
+from lightbulb import Context
+from hikari import Event
+
+# Methods to be uncommented if need be
+
+# Handles event errors
+# async def on_event_error(e_ctx: EventContext, e: Event):
+#     pass
+
+# Handles command errors
+async def on_command_error(com_ctx: CommandContext, ctx: Context):
+    await ctx.respond(f"` > Command '{com_ctx.params.name}' threw an error :( `")
+
+# Called before a command is ran
+# async def on_command_enter(com_ctx: CommandContext, ctx: Context):
+#     pass
+
+# Called after a command is ran
+# async def on_command_exit(com_ctx: CommandContext, ctx: Context):
 #     pass
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/slash-commands/ping.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/slash-commands/ping.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Imports
-from lightbulb import Context
-from lightbulb.ext.hecate import Option, Properties
-
-# Declaring a 'description' attribute sets the description of the command.
-# Equivalent to:
-# params = Params(description="...", ...)
-description = "Replies with 'Pong!'"
-
-# Declaring an 'options' attribute sets the options of the command.
-# Equivalent to:
-# params = Params(options=[...], ...)
-options = [
-    Option('amount', "Number of times to ping", int)
-]
-
-# Declaring a 'pongs' shared attribute so the two commands work together
-properties = Properties(pongs=0)
-
-# Necessary 'command' method, that takes a Context object as argument.
-# Increments the number of pongs by the 'amount' option, and raises ValueError
-# if it's less than 1 
-async def command(ctx: Context):
-    cur_pongs = ctx.options.amount
-    if cur_pongs < 1:
-        raise ValueError
-    properties.pongs += cur_pongs
+# Imports
+from lightbulb import Context
+from lightbulb.ext.hecate import Option, Properties
+
+# Declaring a 'description' attribute sets the description of the command.
+# Equivalent to:
+# params = Params(description="...", ...)
+description = "Replies with 'Pong!'"
+
+# Declaring an 'options' attribute sets the options of the command.
+# Equivalent to:
+# params = Params(options=[...], ...)
+options = [
+    Option('amount', "Number of times to ping", int)
+]
+
+# Declaring a 'pongs' shared attribute so the two commands work together
+properties = Properties(pongs=0)
+
+# Necessary 'command' method, that takes a Context object as argument.
+# Increments the number of pongs by the 'amount' option, and raises ValueError
+# if it's less than 1 
+async def command(ctx: Context):
+    cur_pongs = ctx.options.amount
+    if cur_pongs < 1:
+        raise ValueError
+    properties.pongs += cur_pongs
     await ctx.respond(f"Pong! x{cur_pongs}" if cur_pongs > 1 else "Pong!")
```

### Comparing `lightbulb_ext_hecate-0.1.5/lightbulb/ext/hecate/template/slash-commands/pong_count.py` & `lightbulb_ext_hecate-0.1.6/lightbulb/ext/hecate/template/slash-commands/pong_count.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Imports
-from lightbulb import Context
-from lightbulb.ext.hecate import Params, Properties
-
-# Declaring command attributes with a 'Params' object.
-# The 'name' attribute or Params kwarg should be set if the command
-# is to have a different name from the file name
-params = Params(
-    description="Returns the number of pongs delivered",
-    name='count'
-)
-
-# Declaring a 'pongs' shared attribute so the two commands work together
-properties = Properties(pongs=0)
-
-# Necessary 'command' method, that takes a Context object as argument.
-# Responds with the number of pongs
-async def command(ctx: Context):
+# Imports
+from lightbulb import Context
+from lightbulb.ext.hecate import Params, Properties
+
+# Declaring command attributes with a 'Params' object.
+# The 'name' attribute or Params kwarg should be set if the command
+# is to have a different name from the file name
+params = Params(
+    description="Returns the number of pongs delivered",
+    name='count'
+)
+
+# Declaring a 'pongs' shared attribute so the two commands work together
+properties = Properties(pongs=0)
+
+# Necessary 'command' method, that takes a Context object as argument.
+# Responds with the number of pongs
+async def command(ctx: Context):
     await ctx.respond(f"{properties.pongs} pongs ponged")
```


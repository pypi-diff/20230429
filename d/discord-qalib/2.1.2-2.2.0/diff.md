# Comparing `tmp/discord-qalib-2.1.2.tar.gz` & `tmp/discord-qalib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.1.2.tar", last modified: Thu Apr 20 22:08:44 2023, max compression
+gzip compressed data, was "discord-qalib-2.2.0.tar", last modified: Sat Apr 29 18:14:18 2023, max compression
```

## Comparing `discord-qalib-2.1.2.tar` & `discord-qalib-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:44.935223 discord-qalib-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:08:44.935223 discord-qalib-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:44.931223 discord-qalib-2.1.2/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:08:44.000000 discord-qalib-2.1.2/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 22:08:44.000000 discord-qalib-2.1.2/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:08:44.000000 discord-qalib-2.1.2/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 22:08:44.000000 discord-qalib-2.1.2/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 22:08:44.000000 discord-qalib-2.1.2/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-20 22:08:33.000000 discord-qalib-2.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:44.931223 discord-qalib-2.1.2/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-20 22:08:33.000000 discord-qalib-2.1.2/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:44.931223 discord-qalib-2.1.2/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:08:44.935223 discord-qalib-2.1.2/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 22:08:18.000000 discord-qalib-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:08:44.935223 discord-qalib-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-20 22:08:33.000000 discord-qalib-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/setup.py
```

### Comparing `discord-qalib-2.1.2/LICENSE` & `discord-qalib-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.2/PKG-INFO` & `discord-qalib-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.1.2
+Version: 2.2.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.2 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.1.2/README.md` & `discord-qalib-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.2/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.2.0/discord_qalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.1.2
+Version: 2.2.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.2 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.1.2/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.2.0/discord_qalib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 discord_qalib.egg-info/SOURCES.txt
 discord_qalib.egg-info/dependency_links.txt
 discord_qalib.egg-info/requires.txt
 discord_qalib.egg-info/top_level.txt
 qalib/__init__.py
 qalib/context.py
 qalib/interaction.py
+qalib/py.typed
 qalib/renderer.py
 qalib/template_engines/__init__.py
 qalib/template_engines/formatter.py
 qalib/template_engines/jinja2.py
 qalib/template_engines/template_engine.py
 qalib/translators/__init__.py
 qalib/translators/deserializer.py
 qalib/translators/factory.py
 qalib/translators/json.py
 qalib/translators/message_parsing.py
-qalib/translators/parser.py
+qalib/translators/templater.py
 qalib/translators/xml.py
```

### Comparing `discord-qalib-2.1.2/pyproject.toml` & `discord-qalib-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.1.2"
+version = "2.2.0"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.1.2/qalib/__init__.py` & `discord-qalib-2.2.0/qalib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 from .template_engines.jinja2 import Jinja2
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
-    template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
+        template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
 ) -> Callable[[Callable[..., Coro[T]]], Callable[..., Coro[T]]]:
     """This decorator is used to create a QalibContext object, and pass it to the function as it's first argument,
     overriding the default context.
 
     Args:
         template_engine (TemplateEngine): template engine that is used to template the document
         filename (str): filename of the document
@@ -42,15 +42,14 @@
 
     Returns (QalibContext): decorated function that takes the Context object and using the extended QalibContext object
     """
     renderer_instance: Renderer[str] = Renderer(template_engine, filename, *renderer_options)
 
     def command(func: Callable[..., Coro[T]]) -> Callable[..., Coro[T]]:
         if discord.utils.is_inside_class(func):
-
             @wraps(func)
             async def method(self: commands.Cog, ctx: commands.Context, *args: Any, **kwargs: Any) -> T:
                 return await func(self, QalibContext(ctx, renderer_instance), *args, **kwargs)
 
             return method
 
         @wraps(func)
@@ -59,15 +58,15 @@
 
         return function
 
     return command
 
 
 def qalib_interaction(
-    template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
+        template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
 ) -> Callable[[Callable[..., Coro[T]]], Callable[..., Coro[T]]]:
     """This decorator is used to create a QalibInteraction object, and pass it to the function as it's first argument,
     overriding the default interaction.
 
     Args:
         template_engine (TemplateEngine): template engine that is used to template the document
         filename (str): filename of the document
@@ -76,21 +75,20 @@
     Returns (Callable): decorated function that takes the Interaction object and using the extended
     QalibInteraction object
     """
     renderer_instance: Renderer[str] = Renderer(template_engine, filename, *renderer_options)
 
     def command(func: Callable[..., Coro[T]]) -> Callable[..., Coro[T]]:
         if discord.utils.is_inside_class(func):
-
             @wraps(func)
             async def method(
-                self: commands.Cog,
-                inter: discord.Interaction,
-                *args: Any,
-                **kwargs: Any,
+                    self: commands.Cog,
+                    inter: discord.Interaction,
+                    *args: Any,
+                    **kwargs: Any,
             ) -> T:
                 return await func(self, QalibInteraction(inter, renderer_instance), *args, **kwargs)
 
             return method
 
         @wraps(func)
         async def function(inter: discord.Interaction, *args: Any, **kwargs: Any) -> T:
```

### Comparing `discord-qalib-2.1.2/qalib/context.py` & `discord-qalib-2.2.0/qalib/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import warnings
 from typing import Any, Dict, Generic, Optional
 
 import discord.ext.commands
 import discord.message
+from deprecated import deprecated
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.parser import K
+from qalib.translators.deserializer import K_contra
 
 
-class QalibContext(discord.ext.commands.context.Context, Generic[K]):
+class QalibContext(discord.ext.commands.context.Context, Generic[K_contra]):
     """QalibContext object is responsible for handling messages that are to be sent to the client."""
 
-    def __init__(self, ctx: discord.ext.commands.context.Context, renderer: Renderer[K]):
+    def __init__(self, ctx: discord.ext.commands.context.Context, renderer: Renderer[K_contra]):
         """Constructor for the QalibContext object
 
         Args:
             ctx (commands.context): context object that is passed to the command
             renderer (RendererProxy): renderer object that is used to render the embeds and views
         """
         super().__init__(
@@ -50,100 +52,85 @@
         return message.author == self.message.author and message.channel == self.message.channel
 
     async def get_message(self) -> Optional[str]:
         """This method waits for a message to be sent by the user"""
         confirm: Optional[discord.message.Message] = await self.bot.wait_for("message", timeout=59.0, check=self.verify)
         return confirm.content if confirm is not None else None
 
-    def _render(
-        self,
-        identifier: K,
-        callables: Optional[Dict[str, Callback]] = None,
-        keywords: Optional[Dict[str, Any]] = None,
-        timeout: int = 180,
-    ) -> Message:
-        """This method renders the embed and the view based on the identifier string given.
-
-        Args:
-            identifier (K): identifies the embed in the route file
-            callables (Optional[Dict[str, Callback]]): item callbacks
-            keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
-
-        Returns (Display): tuple of the embed and the view
-        """
-        return self._renderer.render(identifier, callables, keywords, timeout=timeout)
-
     async def rendered_send(
-        self,
-        identifier: K,
-        callables: Optional[Dict[str, Callback]] = None,
-        keywords: Optional[Dict[str, Any]] = None,
-        timeout: int = 180,
-        **kwargs,
+            self,
+            identifier: K_contra,
+            callables: Optional[Dict[str, Callback]] = None,
+            keywords: Optional[Dict[str, Any]] = None,
+            **kwargs,
     ) -> discord.message.Message:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
-            timeout (int): timeout for the view
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._render(identifier, callables, keywords, timeout)
+        message = self._renderer.render(identifier, callables, keywords)
+        assert isinstance(message, Message)
         return await self.send(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def display(
-        self,
-        key: K,
-        callables: Optional[Dict[str, Callback]] = None,
-        keywords: Optional[Dict[str, Any]] = None,
-        timeout: int = 180,
-        **kwargs,
+            self,
+            key: K_contra,
+            callables: Optional[Dict[str, Callback]] = None,
+            keywords: Optional[Dict[str, Any]] = None,
+            **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (str): identifies the embed in the route file
             callables: callable coroutines that are called when the user interacts with the message
             keywords: keywords that are passed to the embed renderer to format the text
-            timeout (int): timeout for the view
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._render(key, callables, keywords, timeout)
+        message = self._renderer.render(key, callables, keywords)
+        assert isinstance(message, Message)
+        if self._displayed:
+            await self._display(**{**message.convert_to_context_message().as_edit().dict(), **kwargs})
+            return
         await self._display(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
         """This method is responsible for sending the message to the client and keeping track of the message object.
 
         Args:
             **kwargs (Dict[str, Any]): kwargs that are passed to the context's send method
         """
         if self._displayed is None:
             self._displayed = await self.send(**kwargs)
         else:
             await self._displayed.edit(**kwargs)
 
+    @deprecated(version="2.1.2", reason="Use rendered_send method instead")
     async def menu(
-        self,
-        key: K,
-        callbacks: Optional[Dict[str, Callback]] = None,
-        keywords: Optional[Dict[str, Any]] = None,
-        **kwargs,
+            self,
+            key: K_contra,
+            callbacks: Optional[Dict[str, Callback]] = None,
+            keywords: Optional[Dict[str, Any]] = None,
+            **kwargs,
     ) -> None:
         """This method is used to create a menu for the user to select from.
 
         Args:
             key (K): identifies the menu in the template file
             callbacks (Dict[str, Callback]): callbacks that are called when the user interacts with the menu
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             **kwargs: kwargs that are passed to the context's send method
         """
-        display = self._renderer.render_menu(key, callbacks=callbacks, keywords=keywords, **kwargs)
+        warnings.warn("use rendered_send method instead", DeprecationWarning)
+        display = self._renderer.render(key, callbacks=callbacks, keywords=keywords)
+        assert isinstance(display, Message)
         await self._display(**{**display.convert_to_context_message().dict(), **kwargs})
```

### Comparing `discord-qalib-2.1.2/qalib/interaction.py` & `discord-qalib-2.2.0/qalib/interaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import warnings
 from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, cast
 
 import discord
+from deprecated import deprecated
 from discord.interactions import InteractionResponse
+from discord.ui import Modal
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.parser import K
+from qalib.translators.deserializer import K_contra
 
 if TYPE_CHECKING:
     from discord.types.interactions import Interaction as InteractionPayload
 
 
 def create_interaction_payload(interaction: discord.Interaction) -> Dict[str, Any]:
     # pylint: disable=protected-access
@@ -25,20 +28,20 @@
         "application_id": interaction.application_id,
         "locale": interaction.locale,
         "guild_locale": interaction.guild_locale,
         "app_permissions": interaction._app_permissions,
     }
 
 
-class QalibInteraction(discord.Interaction, Generic[K]):
+class QalibInteraction(discord.Interaction, Generic[K_contra]):
     """The QalibInteraction class is a subclass of discord.Interaction, and is used to add additional functionality to
     the interaction. It is meant to be used in the on_interaction event, and is responsible for deserializing the
     requested modal and sending it to the user."""
 
-    def __init__(self, interaction: discord.Interaction, renderer: Renderer[K]):
+    def __init__(self, interaction: discord.Interaction, renderer: Renderer[K_contra]):
         """Constructor method for the QalibInteraction class."""
         data = create_interaction_payload(interaction)
         if TYPE_CHECKING:
             super().__init__(
                 data=(cast(InteractionPayload, data)),
                 state=interaction._state,
             )
@@ -48,106 +51,66 @@
                 state=interaction._state,
             )
         self.message = interaction.message
         self.user = interaction.user
         self._renderer = renderer
         self._displayed = False
 
-    async def respond_with_modal(
-            self,
-            key: K,
-            methods: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-    ) -> None:
-        """Method that is responsible for templating the document, and then deserializing the requested modal based on
-        its key and sending it to the user.
-
-        Args:
-            methods (Dict[str, Callback]): methods that are used to override the default methods of the modal
-            key (str): key that identifies the modal in the route file
-            keywords (Any): keywords that are passed to the modal renderer to format the text
-        """
-        if methods is None:
-            methods = {}
-
-        if keywords is None:
-            keywords = {}
-
-        assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
-        # pylint: disable= no-member
-        modal = self._renderer.render_modal(key, methods, keywords)
-        return await self.response.send_modal(modal)  # pyright: ignore [reportGeneralTypeIssues]
-
-    def _render(
-            self,
-            identifier: K,
-            callables: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: int = 180,
-    ) -> Message:
-        """This method renders the embed and the view based on the identifier string given.
-
-        Args:
-            identifier (K): identifies the embed in the route file
-            callables (Optional[Dict[str, Callback]]): item callbacks
-            keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
-
-        Returns (Display): tuple of the embed and the view
-        """
-        return self._renderer.render(identifier, callables, keywords, timeout=timeout)
-
     async def rendered_send(
             self,
-            identifier: K,
+            identifier: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            timeout: int = 180,
             **kwargs,
     ) -> None:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._render(identifier, callables, keywords, timeout)
-
-        assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
-        # pylint: disable= no-member
-        message_info = {**message.convert_to_interaction_message().dict(), **kwargs}
-        return await self.response.send_message(**message_info)  # pyright: ignore [reportGeneralTypeIssues]
+        message = self._renderer.render(identifier, callables, keywords)
+        if isinstance(message, Message):
+            assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
+            # pylint: disable= no-member
+            message_info = {**message.convert_to_interaction_message().dict(), **kwargs}
+            return await self.response.send_message(**message_info)  # pyright: ignore [reportGeneralTypeIssues]
+        if isinstance(message, Modal):
+            assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
+            # pylint: disable= no-member
+            return await self.response.send_modal(message)  # pyright: ignore [reportGeneralTypeIssues]
 
     async def display(
             self,
-            key: K,
+            key: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            timeout: int = 180,
             **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (K): identifies the message in the template file
             callables: callable coroutines that are called when the user interacts with the message
             keywords: keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        message = self._render(key, callables, keywords, timeout)
+        message = self._renderer.render(key, callables, keywords)
+        assert isinstance(message, Message)
+        if self._displayed:
+            await self._display(**{**message.convert_to_interaction_message().as_edit().dict(), **kwargs})
+            return
         await self._display(**{**message.convert_to_interaction_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
         """This method is responsible for sending the message to the client, and editing the message if there is one
         that has already been sent.
 
         Args:
@@ -157,24 +120,43 @@
             await self.edit_original_response(**kwargs)
         else:
             assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
             # pylint: disable= no-member
             await self.response.send_message(**kwargs)  # pyright: ignore [reportGeneralTypeIssues]
             self._displayed = True
 
+    @deprecated(version="2.1.2", reason="Use rendered_send method instead")
     async def menu(
             self,
-            key: K,
+            key: K_contra,
             callbacks: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
             **kwargs,
     ) -> None:
         """This method is used to create a menu for the user to select from.
 
         Args:
             key (K): identifies the menu in the template file
             callbacks (Dict[str, Callback]): callbacks that are called when the user interacts with the menu
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             **kwargs: kwargs that are passed to the context's send method
         """
-        message = self._renderer.render_menu(key, callbacks=callbacks, keywords=keywords, **kwargs)
-        await self._display(**{**message.convert_to_interaction_message().dict(), **kwargs})
+        warnings.warn("Use rendered_send method instead", DeprecationWarning)
+        await self.rendered_send(key, callbacks, keywords, **kwargs)
+
+    @deprecated(version="2.1.2", reason="Use rendered_send method instead")
+    async def respond_with_modal(
+            self,
+            key: K_contra,
+            methods: Optional[Dict[str, Callback]] = None,
+            keywords: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """Method that is responsible for templating the document, and then deserializing the requested modal based on
+        its key and sending it to the user.
+
+        Args:
+            methods (Dict[str, Callback]): methods that are used to override the default methods of the modal
+            key (str): key that identifies the modal in the route file
+            keywords (Any): keywords that are passed to the modal renderer to format the text
+        """
+        warnings.warn("Use rendered_send method instead", DeprecationWarning)
+        await self.rendered_send(key, methods, keywords)
```

### Comparing `discord-qalib-2.1.2/qalib/template_engines/formatter.py` & `discord-qalib-2.2.0/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.2/qalib/template_engines/jinja2.py` & `discord-qalib-2.2.0/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.2/qalib/translators/__init__.py` & `discord-qalib-2.2.0/qalib/translators/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,136 @@
-import dataclasses
-from dataclasses import dataclass
-from typing import Any, Awaitable, Callable, Dict, Optional, Sequence, TypeVar, Union
+from dataclasses import dataclass, fields
+from typing import Any, Awaitable, Callable, Dict, Optional, Sequence, TypeVar, Union, TypedDict
 
 import discord
 from discord.abc import Snowflake
+from typing_extensions import ParamSpec
 
 V_co = TypeVar("V_co", bound=discord.ui.View, covariant=True)
 
+M = TypeVar("M")
+N = TypeVar("N")
+P = ParamSpec("P")
+
 Callback = Callable[[discord.Interaction], Awaitable[None]]
 CallbackMethod = Callable[[discord.ui.Item[V_co], discord.Interaction], Awaitable[None]]
 
 
 @dataclass
 class DiscordIdentifier(Snowflake):
     # pylint: disable=invalid-name
     id: int
 
 
 @dataclass
-class BaseMessage:
+class Base:
+    def dict(self) -> Dict[str, Any]:
+        return {key.name: attr for key in fields(self) if (attr := getattr(self, key.name)) is not None}
+
+
+@dataclass
+class BaseEditMessage(Base):
+    content: Optional[str]
+    embed: Optional[discord.Embed]
+    attachments: Optional[Sequence[Union[discord.Attachment, discord.File]]]
+    delete_after: Optional[float]
+    allowed_mentions: Optional[discord.AllowedMentions]
+    view: Optional[discord.ui.View]
+
+
+# pylint: disable= too-many-instance-attributes
+@dataclass
+class BaseMessage(Base):
     content: Optional[str]
     embed: Optional[discord.Embed]
     embeds: Optional[Sequence[discord.Embed]]
     file: Optional[discord.File]
     files: Optional[Sequence[discord.File]]
     view: Optional[discord.ui.View]
     tts: Optional[bool]
     ephemeral: Optional[bool]
     allowed_mentions: Optional[discord.AllowedMentions]
     suppress_embeds: Optional[bool]
-    silent: Optional[bool]
     delete_after: Optional[float]
 
-    def dict(self) -> Dict[str, Any]:
-        return {key.name: attr for key in dataclasses.fields(self) if (attr := getattr(self, key.name)) is not None}
+    def as_edit(self) -> BaseEditMessage:
+        raise NotImplementedError
+
 
-    def __iter__(self):
-        # Order is preserved in Python 3.7+: https://mail.python.org/pipermail/python-dev/2017-December/151283.html
-        for key in dataclasses.fields(self):
-            value = getattr(self, key.name)
-            if value is None:
-                continue
-            yield value
+@dataclass
+class EditContextMessage(BaseEditMessage):
+    suppress: Optional[bool]
 
 
 @dataclass
 class ContextMessage(BaseMessage):
     stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]]
     nonce: Optional[Union[str, int]]
     reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]]
     mention_author: Optional[bool]
 
+    def as_edit(self) -> EditContextMessage:
+        return EditContextMessage(
+            content=self.content,
+            embed=self.embed,
+            attachments=self.files,
+            suppress=self.suppress_embeds,
+            delete_after=self.delete_after,
+            allowed_mentions=self.allowed_mentions,
+            view=self.view
+        )
+
+
+@dataclass
+class InteractionEditMessage(BaseEditMessage):
+    pass
+
 
 @dataclass
 class InteractionMessage(BaseMessage):
     silent: Optional[bool]
 
+    def as_edit(self) -> InteractionEditMessage:
+        return InteractionEditMessage(
+            content=self.content,
+            embed=self.embed,
+            attachments=self.files,
+            delete_after=self.delete_after,
+            allowed_mentions=self.allowed_mentions,
+            view=self.view
+        )
+
+
+class MessageTyped(TypedDict):
+    content: Optional[str]
+    embed: Optional[discord.Embed]
+    embeds: Optional[Sequence[discord.Embed]]
+    file: Optional[discord.File]
+    files: Optional[Sequence[discord.File]]
+    view: Optional[discord.ui.View]
+    tts: Optional[bool]
+    ephemeral: Optional[bool]
+    allowed_mentions: Optional[discord.AllowedMentions]
+    suppress_embeds: Optional[bool]
+    silent: Optional[bool]
+    delete_after: Optional[float]
+    stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]]
+    nonce: Optional[Union[str, int]]
+    reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]]
+    mention_author: Optional[bool]
+
 
 # pylint: disable=too-many-instance-attributes
 @dataclass
 class Message(BaseMessage):
     """Dataclass that represents the display of the message.
 
     Look at https://discordpy.readthedocs.io/en/latest/api.html?highlight=send#discord.abc.Messageable.send
     """
+
     stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]]
     nonce: Optional[Union[str, int]]
     reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]]
     mention_author: Optional[bool]
     silent: Optional[bool]
 
     def convert_to_context_message(self) -> ContextMessage:
@@ -78,15 +141,14 @@
             file=self.file,
             files=self.files,
             view=self.view,
             tts=self.tts,
             ephemeral=self.ephemeral,
             allowed_mentions=self.allowed_mentions,
             suppress_embeds=self.suppress_embeds,
-            silent=self.silent,
             delete_after=self.delete_after,
             stickers=self.stickers,
             nonce=self.nonce,
             reference=self.reference,
             mention_author=self.mention_author,
         )
 
@@ -101,7 +163,10 @@
             tts=self.tts,
             ephemeral=self.ephemeral,
             allowed_mentions=self.allowed_mentions,
             suppress_embeds=self.suppress_embeds,
             silent=self.silent,
             delete_after=self.delete_after,
         )
+
+    def as_edit(self) -> InteractionEditMessage:
+        raise NotImplementedError
```

### Comparing `discord-qalib-2.1.2/qalib/translators/factory.py` & `discord-qalib-2.2.0/qalib/translators/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-from typing import Any, Optional, Type, cast
+from typing import Optional, Type, cast, Literal, Dict
 
 from .deserializer import Deserializer
-from .json import JSONDeserializer, JSONParser
-from .parser import Parser
-from .xml import XMLDeserializer, XMLParser
+from .json import JSONDeserializer, JSONTemplater
+from .templater import Templater
+from .xml import XMLDeserializer, XMLTemplater
 
+Extensions = Literal[".xml", ".json"]
 
-class ParserFactory:
+
+class TemplaterFactory:
     """Factory class for creating Parsers"""
 
-    parsers = {".xml": XMLParser, ".json": JSONParser}
+    parsers: Dict[Extensions, Type[Templater]] = {".xml": XMLTemplater, ".json": JSONTemplater}
 
     @staticmethod
-    def get_parser_type(path: str) -> Type[Parser[str]]:
+    def get_templater_type(path: str) -> Type[Templater]:
         """Returns the parser type based on the file extension of the path.
 
         Args:
             path (str): path of the file that is parsed
 
         Returns (Type[Parser]): parser type that is used to parse the file
         """
-        for extension, parser_type in ParserFactory.parsers.items():
+        for extension, parser_type in TemplaterFactory.parsers.items():
             if path.endswith(extension):
-                return cast(Type[Parser[Any]], parser_type)
+                return cast(Type[Templater], parser_type)
 
         raise ValueError("No parser found for the given file")
 
     @staticmethod
-    def get_parser(path: str, *, source: Optional[str] = None) -> Parser[str]:
+    def get_templater(path: str, *, source: Optional[str] = None) -> Templater:
         """Returns an instantiated Parser based on the file extension of the path using either the source contents or
         the path.
 
         Args:
             path (str): path of the file that is parsed
             source (Optional[str]): source contents that are parsed
 
         Returns (Parser): parser that is used to parse the file
         """
-        parser = ParserFactory.get_parser_type(path)
+        parser = TemplaterFactory.get_templater_type(path)
         if source is not None:
             return parser(source=source)
         with open(path, encoding="utf8", mode="r") as file:
             return parser(source=file.read())
 
 
 class DeserializerFactory:
     """Factory class for creating Deserializers"""
 
-    deserializers = {".xml": XMLDeserializer, ".json": JSONDeserializer}
+    deserializers: Dict[Extensions, Type[Deserializer[str]]] = {".xml": XMLDeserializer, ".json": JSONDeserializer}
 
     @staticmethod
-    def get_deserializer_type(path: str) -> Type[Deserializer]:
+    def get_deserializer_type(path: str) -> Type[Deserializer[str]]:
         """This function returns the correct translators for the given file.
 
         Args:
             path (str): path to the file
 
         Returns (Deserializer): th deserializer for the given file
         """
         for extension, deserializer_type in DeserializerFactory.deserializers.items():
             if path.endswith(extension):
                 return deserializer_type
 
         raise ValueError("No deserializer found for the given file")
 
     @staticmethod
-    def get_deserializer(path: str) -> Deserializer:
+    def get_deserializer(path: str) -> Deserializer[str]:
         """This static method returns the deserializer based on the given path's file extension.
 
         Args:
             path (str): path to the file
 
         Returns (Deserializer): deserializer for the given file
         """
```

### Comparing `discord-qalib-2.1.2/qalib/translators/json.py` & `discord-qalib-2.2.0/qalib/translators/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import json
 from copy import deepcopy
 from datetime import datetime
 from functools import partial
-from typing import Any, Callable, Dict, List, Literal, Optional, Type, TypedDict, TypeVar, Union, cast
+from typing import Any, Callable, Dict, List, Literal, Optional, Type, TypedDict, TypeVar, Union, cast, Tuple, Sequence
 
 import discord
 import discord.types.embed
 from discord import ui
 from discord.abc import Snowflake
 from typing_extensions import NotRequired
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer
+from qalib.translators.deserializer import Deserializer, ElementTypes, Types, ReturnType, K_contra
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ButtonStyle,
     ChannelType,
     CustomSelects,
     Emoji,
     create_button,
@@ -30,16 +30,17 @@
     make_colour,
     make_emoji,
     Field,
     Footer,
     Author,
     TextInputRaw,
     TextInputComponent,
+    make_expansive_embeds, apply, bind_menu, attach_views
 )
-from qalib.translators.parser import K, Parser
+from qalib.translators.templater import Templater
 
 OBJ = TypeVar("OBJ")
 
 ComponentTypes = Literal[
     "button",
     "select",
     "channel_select",
@@ -110,41 +111,44 @@
     row: NotRequired[int]
 
 
 class TextInput(TextInputRaw):
     type: ComponentTypes
 
 
-Components = Union[Button, Select, CustomSelect, ChannelSelect, TextInput]
+ComponentType = Union[Button, Select, CustomSelect, ChannelSelect, TextInput]
+Components = Dict[str, ComponentType]
 
 
 class Timestamp(TypedDict):
     """This class is used to represent object's timestamp."""
 
     date: str
     format: NotRequired[str]
 
 
 class Embed(TypedDict):
-    """This class is used to represent the blueprint of an embed."""
-
     title: str
     colour: NotRequired[str]
     color: NotRequired[str]
     fields: List[Field]
     description: NotRequired[str]
     type: NotRequired[discord.types.embed.EmbedType]
     url: NotRequired[str]
     timestamp: NotRequired[Timestamp]
     footer: NotRequired[Footer]
     image: NotRequired[str]
     thumbnail: NotRequired[str]
     author: NotRequired[Author]
 
 
+class ExpansiveEmbed(Embed):
+    expansive_field: Field
+
+
 class File(TypedDict):
     """This class is used to represent the blueprint of a file."""
 
     filename: str
     spoiler: NotRequired[bool]
     description: NotRequired[str]
 
@@ -162,48 +166,69 @@
     """This class is used to represent the blueprint of a message reference."""
 
     message_id: int
     channel_id: int
     guild_id: NotRequired[int]
 
 
-View = Dict[str, Components]
+class View(TypedDict):
+    timeout: NotRequired[Optional[float]]
+    components: Components
 
 
-class JSONMessage(TypedDict):
-    """This class is used to represent the blueprint of a message."""
+class Element(TypedDict):
+    type: Types
 
-    embed: NotRequired[Embed]
-    embeds: NotRequired[List[Embed]]
+
+class BaseMessage(Element):
     view: NotRequired[View]
+    timeout: NotRequired[float]
     content: NotRequired[str]
+    embeds: NotRequired[List[Embed]]
     tts: NotRequired[bool]
     nonce: NotRequired[int]
     delete_after: NotRequired[float]
     suppress_embeds: NotRequired[bool]
     file: NotRequired[File]
     files: NotRequired[List[File]]
     allowed_mentions: NotRequired[AllowedMentions]
     message_reference: NotRequired[MessageReference]
     mention_author: NotRequired[bool]
+    ephemeral: NotRequired[bool]
     silent: NotRequired[bool]
 
 
-JSONMenu = Dict[str, JSONMessage]
+class RegularMessage(BaseMessage):
+    """This class is used to represent the blueprint of a message."""
+    embed: NotRequired[Embed]
+
+
+class ExpansiveMessage(BaseMessage):
+    page_number_key: NotRequired[str]
+    embed: ExpansiveEmbed
+
+
+Page = Union[RegularMessage, ExpansiveMessage]
 
 
-class JSONModal(TypedDict):
+class Menu(Element):
+    timeout: NotRequired[Optional[float]]
+    pages: List[Union[str, Page]]
+
+
+class Modal(Element):
     title: str
-    components: Dict[str, Components]
+    components: Components
 
 
-Template = Dict[str, Union[JSONMessage, JSONMenu, JSONModal]]
+Elements = Union[RegularMessage, ExpansiveMessage, Menu, Modal]
+Document = Dict[str, Elements]
 
 
-class JSONParser(Parser[K]):
+class JSONTemplater(Templater):
     """This method is used to parse the document into a menu and a list of callables for .json files"""
 
     __slots__ = ("_data",)
 
     def __init__(self, source: str):
         """This method is used to initialize the parser by parsing the source text.
 
@@ -229,162 +254,210 @@
             for i, value in enumerate(obj):
                 obj[i] = self.recursive_template(value, template_engine, keywords)
         elif isinstance(obj, str):
             return cast(OBJ, template_engine.template(obj, keywords))
 
         return obj
 
-    def template_message(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """This method is used to template the embed by first retrieving it using its key, and then templating it using
-        the template_engine
+    def template(self, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+        """This method is used to template the element by first retrieving it using its key, and then templating it
+        using the template_engine
 
         Args:
-            key (K): key of the embed
-            template_engine (TemplateEngine): template engine that is used to template the embed
-            keywords (Dict[str, Any]): keywords that are used to template the embed
+            template_engine (TemplateEngine): template engine that is used to template the element
+            keywords (Dict[str, Any]): keywords that are used to template the element
 
-        Returns (str): templated embed in the form of string.
+        Returns (str): templated element in the form of string.
         """
-        return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
+        return json.dumps(self.recursive_template(deepcopy(self._data), template_engine, keywords))
 
-    def template_menu(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """Method that is used to template the menu by first retrieving it using its key, and then templating it using
-        the template_engine
 
-        Args:
-            key (K): key of the menu
-            template_engine (TemplateEngine): template engine that is used to template the menu
-            keywords (Dict[str, Any]): keywords that are used to template the menu
+class JSONDeserializer(Deserializer[K_contra]):
 
-        Returns (str): templated menu in the form of string.
-        """
-        return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
-
-    def template_modal(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """Method that is used to template the modal by first retrieving it using its key, and then templating it using
-        the template_engine
+    def deserialize(self, source: str, key: K_contra, callables: Dict[str, Callback]) -> ReturnType:
+        """Method to deserialize a source into a Display object
 
         Args:
-            key (K): key of the modal
-            template_engine (TemplateEngine): template engine that is used to template the modal
-            keywords (Dict[str, Any]): keywords that are used to template the modal
+            source (str): The source text to deserialize
+            key (K): The key of the element to deserialize
+            callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
 
-        Returns (str): templated modal in the form of string.
+        Returns (ReturnType): All possible deserialized objects.
         """
-        return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
-
+        document: Document = json.loads(source)
+        element: Elements = document[key]
+        return self.deserialize_element(document, element, callables)
 
-class JSONDeserializer(Deserializer):
-    def deserialize_into_message(self, source: str, callables: Dict[str, Callback], **kw) -> Message:
-        """Method to deserialize a source into a Display object
+    def deserialize_element(self, document: Document, element: Elements, callables: Dict[str, Callback]) -> ReturnType:
+        """Method to deserialize an element into a Display object
 
         Args:
-            source (str): The source text to deserialize
+            document (Document): The document to deserialize
+            element (Elements): The element to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            **kw: Additional keyword arguments
 
-        Returns (Display): A Display object
+        Returns (ReturnType): All possible deserialized objects.
         """
-        return self.deserialize_message(json.loads(source), callables, kw)
+        element_type: Optional[ElementTypes] = ElementTypes.from_str(element["type"])
+
+        deserializers: Dict[ElementTypes, Callable[..., ReturnType]] = {
+            ElementTypes.MESSAGE: self.deserialize_message,
+            ElementTypes.EXPANSIVE: bind_menu(self.deserialize_expansive),
+            ElementTypes.MENU: bind_menu(partial(self.deserialize_menu, document=document)),
+            ElementTypes.MODAL: self.deserialize_modal,
+        }
+        assert element_type is not None, f"Invalid element type: {element['type']}"
+        return deserializers[element_type](element, callables)
 
     # pylint: disable= too-many-locals
     def deserialize_message(
-        self,
-        message_tree: JSONMessage,
-        callables: Dict[str, Callback],
-        kwargs: Dict[str, Any],
+            self,
+            message_tree: Union[RegularMessage, ExpansiveMessage],
+            callables: Dict[str, Callback],
+            **overrides: Any
     ) -> Message:
         """Method to deserialize an embed into a Display NamedTuple containing the embed and the view
 
         Args:
             message_tree (Dict[str, Any]): The embed to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kwargs (Dict[str, Any]): A dictionary containing the attributes to use for the view
+            **overrides (Any): keyword arguments that override the messages
 
         Returns (Display): A Display NamedTuple containing the embed and the view
         """
-        view_tree = message_tree.get("view")
-        embed = self.render(embed_tree) if (embed_tree := message_tree.get("embed")) is not None else None
-        view = None if view_tree is None else self._render_view(view_tree, callables, kwargs)
-        return Message(
-            embed=embed,
-            embeds=None if (embeds := message_tree.get("embeds")) is None else list(map(self.render, embeds)),
-            content=message_tree.get("content", None),
-            tts=None
-            if (tts_element := message_tree.get("tts")) is None
-            else ((isinstance(tts_element, bool) and tts_element) or str(tts_element).lower() == "true"),
-            nonce=None if (nonce_element := message_tree.get("nonce")) is None else int(nonce_element),
-            delete_after=None if (delete_after := message_tree.get("delete_after")) is None else float(delete_after),
-            suppress_embeds=None if (suppress := message_tree.get("suppress_embeds")) is None else suppress,
-            file=None if (file := message_tree.get("file")) is None else self._render_file(file),
-            files=None if (files := message_tree.get("files")) is None else list(map(self._render_file, files)),
-            allowed_mentions=None
-            if (allowed_mentions := message_tree.get("allowed_mentions")) is None
-            else self._render_allowed_mentions(allowed_mentions),
-            reference=None
-            if (reference := message_tree.get("message_reference")) is None
-            else discord.MessageReference(
+
+        def render(embeds: List[Embed]) -> Sequence[discord.Embed]:
+            return [self._render_embed(embed) for embed in embeds]
+
+        message = Message(
+            embed=apply(message_tree.get("embed"), self._render_embed),
+            embeds=apply(message_tree.get("embeds"), render),
+            content=message_tree.get("content"),
+            tts=message_tree.get("tts"),
+            nonce=apply(message_tree.get("nonce"), int),
+            delete_after=apply(message_tree.get("delete_after"), float),
+            suppress_embeds=message_tree.get("suppress_embeds"),
+            file=apply(message_tree.get("file"), self._render_file),
+            files=apply(message_tree.get("files"), lambda files: list(map(self._render_file, files))),
+            allowed_mentions=apply(message_tree.get("allowed_mentions"), self._render_allowed_mentions),
+            reference=apply(message_tree.get("message_reference"), lambda reference: discord.MessageReference(
                 message_id=reference["message_id"],
                 channel_id=reference["channel_id"],
                 guild_id=reference.get("guild_id"),
-            ),
+            )),
             mention_author=message_tree.get("mention_author"),
-            view=view,
+            view=apply(message_tree.get("view"), self._render_view, callables),
             stickers=None,
-            ephemeral=None,
-            silent=message_tree.get("silent")
+            ephemeral=message_tree.get("ephemeral"),
+            silent=message_tree.get("silent"),
         )
 
-    def deserialize_into_menu(self, source: str, callables: Dict[str, Callback], **kw) -> List[Message]:
-        """Method to deserialize a menu into a list of Display objects
+        for key, value in overrides.items():
+            setattr(message, key, value)
+
+        return message
+
+    def deserialize_expansive(self, message_tree: ExpansiveMessage, callbacks: Dict[str, Callback]) -> List[Message]:
+        """Method to deserialize a source into a list of Display objects
 
         Args:
-            source (str): The source text to deserialize int a Menu
-            callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            **kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
+            message_tree (ExpansiveMessage): The ExpansiveMessage of the message_tree
+            callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
 
         Returns (List[Display]): A list of Display objects
         """
-        return [self.deserialize_message(embed, callables, kw) for embed in json.loads(source).values()]
+        timeout = 180.0
+        if "timeout" in message_tree:
+            timeout = message_tree["timeout"]
+        messages = [self.deserialize_message(message_tree, callbacks, embed=embed)
+                    for embed in self._separate_embed(message_tree["embed"], message_tree.get("page_number_key"))]
+
+        attach_views(messages, timeout)
+        return messages
+
+    def deserialize_page(
+            self,
+            document: Document,
+            raw_page: Union[str, Page],
+            callables: Dict[str, Callback]
+    ) -> List[Message]:
+        """Method to deserialize a page into a Display object
 
-    def deserialize_into_modal(self, source: str, methods: Dict[str, Callback], **kw: Any) -> discord.ui.Modal:
-        """Method to deserialize a modal into a discord.ui.Modal object
+        Args:
+            document (Document): the original document containing all the keys.
+            raw_page (Page): The page to deserialize
+            callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+
+        Returns (Display): A Display object
+        """
+        page = document[raw_page] if isinstance(raw_page, str) else raw_page
+        element_type = ElementTypes.from_str(page["type"])
+        if element_type == ElementTypes.MESSAGE:
+            return [self.deserialize_message(cast(RegularMessage, page), callables)]
+        if element_type == ElementTypes.EXPANSIVE:
+            return self.deserialize_expansive(cast(ExpansiveMessage, page), callables)
+        raise TypeError(f"Invalid type {element_type} for page")
+
+    def deserialize_menu(self, menu: Menu, callables: Dict[str, Callback], *, document: Document) -> List[Message]:
+        """Method to deserialize a menu into a list of Display objects
 
         Args:
-            source (str): The source text to deserialize into a modal
-            methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            **kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
+            menu (Menu): The Menu Dictionary to deserialize into a List of Messages
+            callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            document (Document): the original document containing all the keys.
 
-        Returns (discord.ui.Modal): A discord.ui.Modal object
+        Returns (List[Message]): A list of Display objects
         """
-        modal_tree = json.loads(source)
-        return self._render_modal(modal_tree, methods, kw)
+        pages: List[Message] = sum((self.deserialize_page(document, page, callables) for page in menu["pages"]), [])
 
-    def _render_modal(self, tree: JSONModal, methods: Dict[str, Callback], kwargs: Dict[str, Any]) -> discord.ui.Modal:
-        """Method to render a modal from a modal tree
+        timeout: Optional[float] = menu.get("timeout", 180.0)
+
+        for page in pages:
+            if page.view is None:
+                page.view = ui.View(timeout=timeout)
+            else:
+                page.view.timeout = timeout
+        return pages
+
+    def deserialize_modal(self, tree: Modal, methods: Dict[str, Callback]) -> discord.ui.Modal:
+        """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
-            tree (Dict[str, Any]): The modal tree to render
+            tree (Modal): The Modal Dictionary to deserialize into a discord.ui.Modal object
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
-        modal = type(f"{tree['title']} Modal", (discord.ui.Modal,), methods)(title=(tree["title"]), **kwargs)
+        modal = type(f"{tree['title']} Modal", (discord.ui.Modal,), methods)(title=tree["title"])
 
         components = self.render_components(tree["components"]) if "components" in tree else []
 
         for component in components:
             modal.add_item(component)
 
         return modal
 
+    def _separate_embed(self, raw_embed: ExpansiveEmbed, replacement_key: Optional[str]) -> List[discord.Embed]:
+        """Separates the embeds from the raw embed element.
+
+        Args:
+            raw_embed (ElementTree.Element): The raw embed element.
+            replacement_key (str): the key to replace with the page number.
+
+        Returns (List[discord.Embed]): A list of embeds.
+        """
+        return make_expansive_embeds(raw_embed["expansive_field"]["name"],
+                                     raw_embed["expansive_field"]["value"],
+                                     replacement_key,
+                                     raw_embed,
+                                     self._render_embed)
+
     @staticmethod
     def _render_allowed_mentions(
-        allowed_mentions: AllowedMentions,
+            allowed_mentions: AllowedMentions,
     ) -> discord.AllowedMentions:
         def parse_mentions(mentions: Union[bool, List[int]]) -> Union[bool, List[Snowflake]]:
             if isinstance(mentions, bool):
                 return mentions
             return [DiscordIdentifier(int(identifier)) for identifier in mentions]
 
         return discord.AllowedMentions(
@@ -405,26 +478,27 @@
         """
         return discord.File(
             fp=raw_file["filename"],
             description=raw_file["description"] if "description" in raw_file else None,
             spoiler=raw_file["spoiler"] if "spoiler" in raw_file else False,
         )
 
-    def _render_view(self, raw_view: View, callables: Dict[str, Callback], kwargs: Dict[str, Any]) -> ui.View:
+    def _render_view(self, raw_view: View, callables: Dict[str, Callback]) -> ui.View:
         """Method to render a view element into a discord.ui.View object
 
         Args:
             raw_view (View) The view element to render
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kwargs (Dict[str, Any]): A dictionary containing the attributes to use for the view
 
         Returns (ui.View): A discord.ui.View object
         """
-        view = ui.View(**kwargs)
-        for component in self.render_components(raw_view, callables):
+        view = ui.View()
+        if "timeout" in raw_view:
+            view.timeout = raw_view["timeout"]
+        for component in self.render_components(raw_view["components"], callables):
             view.add_item(component)
         return view
 
     @staticmethod
     def _render_timestamp(timestamp: Optional[Timestamp]) -> Optional[datetime]:
         """Method to render a timestamp element into a datetime object
 
@@ -488,17 +562,17 @@
         if "channel_types" in component:
             attributes["channel_types"] = make_channel_types(component["channel_types"])
 
         select: ui.ChannelSelect = create_channel_select(callback=callback, **attributes)
         return select
 
     def _render_select(
-        self,
-        component: Select,
-        callback: Optional[Callback],
+            self,
+            component: Select,
+            callback: Optional[Callback],
     ) -> ui.Select:
         """Renders a select menu from the given component's template
 
         Args:
             component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
             callback (Optional[Callback]): the callback to be called when the select menu is pressed
 
@@ -513,15 +587,15 @@
         attributes["options"] = options
 
         select: ui.Select = create_select(callback=callback, **attributes)
         return select
 
     @staticmethod
     def _render_type_select(
-        select_type: Type[CustomSelects], component: CustomSelect, callback: Optional[Callback]
+            select_type: Type[CustomSelects], component: CustomSelect, callback: Optional[Callback]
     ) -> CustomSelects:
         """Renders a type select menu from the given component's template
 
         Args:
             component (component): the component's template
             callback (Optional[Callback]): the callback to be called it is selected from the select menu
 
@@ -542,17 +616,17 @@
         if callback is not None:
             component["callback"] = callback
 
         text_input: ui.TextInput = create_text_input(component)
         return text_input
 
     def render_component(
-        self,
-        component: Components,
-        callback: Optional[Callback],
+            self,
+            component: ComponentType,
+            callback: Optional[Callback],
     ) -> ui.Item:
         """Renders a component from the given component's template
 
         Args:
             component (Components): the component's template
             callback (Optional[Callback]): the callback to be called when the user interacts with the component
 
@@ -570,54 +644,68 @@
         }
 
         component_type: ComponentTypes = component["type"]
         item_renderer = component_renderer[component_type]
 
         return item_renderer(component, callback)
 
-    def render_components(self, view: View, callables: Optional[Dict[str, Callback]] = None) -> List[ui.Item]:
+    def render_components(
+            self,
+            components: Components,
+            callables: Optional[Dict[str, Callback]] = None
+    ) -> List[ui.Item]:
         """Renders the components specified by the identifier
 
         Args:
-            view (Dict[str, ...]): the dictionary containing the view component.
+            components (Components): the dictionary containing the view component.
             callables (Dict[str, Callback]): the callbacks to be called when the user interacts with the components
 
-        Returns (Optional[List[ui.Item]]): the rendered components
+        Returns (List[ui.Item]): the rendered components
         """
         if callables is None:
             callables = {}
-        return [self.render_component(component, callables.get(key)) for key, component in view.items()]
+        return [self.render_component(component, callables.get(key)) for key, component in components.items()]
 
-    def render(self, raw_embed: Embed) -> discord.Embed:
+    def _render_embed(self, raw_embed: Embed, *replacements: Tuple[str, str]) -> discord.Embed:
         """Render the desired templated embed in discord.Embed instance
 
         Args:
-           raw_embed (Embed): the dictionary containing the required key, values needed to render the
-                                        embed.
+           raw_embed (Embed): the dictionary containing the required key, values needed to render the embed.
+           *replacements (Tuple[str, str]): Replace the first string with the second string in the embed.
 
         Returns:
             discord.Embed: Embed Object, discord compatible.
         """
         assert "colour" in raw_embed or "color" in raw_embed, "Embed must have either a colour or color key"
 
+        def replace(value: Optional[str]) -> Optional[str]:
+            if value is None:
+                return value
+            for replacement in replacements:
+                value = value.replace(*replacement)
+            return value
+
         embed = discord.Embed(
-            title=raw_embed["title"],
+            title=replace(raw_embed["title"]),
             colour=make_colour(raw_embed["colour"] if "colour" in raw_embed else raw_embed["color"]),
             type="rich" if "type" not in raw_embed else raw_embed["type"],
-            url=raw_embed["url"] if "url" in raw_embed else None,
-            description=raw_embed["description"] if "description" in raw_embed else None,
+            url=replace(raw_embed["url"]) if "url" in raw_embed else None,
+            description=replace(raw_embed["description"]) if "description" in raw_embed else None,
             timestamp=self._render_timestamp(raw_embed.get("timestamp")),
         )
 
-        for field in raw_embed["fields"]:
+        for field in raw_embed.get("fields", []):
             embed.add_field(**field)
 
         if "footer" in raw_embed:
-            embed.set_footer(**raw_embed["footer"])
+            embed.set_footer(text=replace(raw_embed["footer"].get("text")),
+                             icon_url=replace(raw_embed["footer"].get("icon_url")))
 
-        embed.set_thumbnail(url=raw_embed.get("thumbnail"))
-        embed.set_image(url=raw_embed.get("image"))
+        embed.set_thumbnail(url=replace(raw_embed.get("thumbnail")))
+        embed.set_image(url=replace(raw_embed.get("image")))
 
         if "author" in raw_embed:
-            embed.set_author(**raw_embed["author"])
+            embed.set_author(name=replace(raw_embed["author"]["name"]),
+                             url=replace(raw_embed["author"]["url"]),
+                             icon_url=replace(raw_embed["author"]["icon_url"]))
 
         return embed
```

### Comparing `discord-qalib-2.1.2/qalib/translators/xml.py` & `discord-qalib-2.2.0/qalib/translators/xml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from datetime import datetime
 from functools import partial
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, TypeVar, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Type, cast, Tuple
 from xml.etree import ElementTree
 
 import discord
 import discord.types.embed as embed_types
 from discord import ui
 from discord.abc import Snowflake
-from typing_extensions import Concatenate, ParamSpec
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer
+from qalib.translators.deserializer import Deserializer, ElementTypes, ReturnType, K_contra
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ChannelType,
     Emoji,
     create_button,
     create_channel_select,
     create_select,
@@ -26,167 +25,145 @@
     make_channel_types,
     make_colour,
     make_emoji,
     Field,
     Footer,
     Author,
     TextInputComponent,
+    make_expansive_embeds, attach_views, apply, bind_menu,
 )
-from qalib.translators.parser import K, Parser
+from qalib.translators.templater import Templater
 
-M = TypeVar("M")
-N = TypeVar("N")
-P = ParamSpec("P")
+
+def get_text(element_tree: ElementTree.Element, child: str) -> Optional[str]:
+    element = element_tree.find(child)
+    if element is None:
+        return None
+    return None if element.text is None else element.text
+
+
+def get_element(element_tree: ElementTree.Element, child: str) -> Optional[ElementTree.Element]:
+    return None if (element := element_tree.find(child)) is None else element
 
 
-class XMLParser(Parser[K]):
+class XMLTemplater(Templater):
     def __init__(self, source: str):
         """Initialisation of the XML Parser
 
         Args:
             source (str): the text of the XML file
         """
+        self.source = source
         self.root = ElementTree.fromstring(source)
 
-    def get_message(self, identifier: K) -> str:
-        """This method is used to get an embed by its key.
-
-        Args:
-            identifier (K): key of the embed
-
-        Returns (str): a raw string containing the embed.
-        """
-        for message in self.root.findall("message"):
-            if message.get("key") == identifier:
-                return ElementTree.tostring(message, encoding="unicode", method="xml")
-        raise KeyError(f"Message with key {identifier} not found")
-
-    def get_menu(self, identifier: K) -> str:
-        """This method is used to get a menu by its key.
-
-        Args:
-            identifier (K): key of the menu
-
-        Returns (str): a raw string containing the menu.
-        """
-        for menu in self.root.findall("menu"):
-            if menu.get("key") == identifier:
-                return ElementTree.tostring(menu, encoding="unicode", method="xml")
-        raise KeyError(f"Menu with key {identifier} not found")
-
-    def get_modal(self, identifier: K) -> str:
-        """This method is used to get a modal by its key.
-
-        Args:
-            identifier (K): key of the modal
-
-        Returns (str): a raw string containing the modal.
-        """
-        for modal in self.root.findall("modal"):
-            if modal.get("key") == identifier:
-                return ElementTree.tostring(modal, encoding="unicode", method="xml")
-        raise KeyError(f"Modal with key {identifier} not found")
-
-    def template_message(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """This method is used to template an embed, by identifying it by its key and using the template engine to
+    def template(self, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+        """This method is used to template an element, by identifying it by its key and using the template engine to
         template it.
 
         Args:
-            key (K): key of the embed
             template_engine (TemplateEngine): template engine that is used to template the embed
             keywords (Dict[str, Any]): keywords that are used to template the embed
 
         Returns (str): templated embed
         """
-        return template_engine.template(self.get_message(key), keywords)
+        return template_engine.template(self.source, keywords)
 
-    def template_menu(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """This method is used to template a menu, by identifying it by its key and using the template engine to
-        template it.
 
-        Args:
-            key (K): key of the menu
-            template_engine (TemplateEngine): template engine that is used to template the menu
-            keywords (Dict[str, Any]): keywords that are used to template the menu
+class XMLDeserializer(Deserializer[K_contra]):
+    """Read and process the data given by the XML file, and use given user objects to render the text"""
 
-        Returns (str): templated menu
-        """
-        return template_engine.template(self.get_menu(key), keywords)
+    def _get_element(self, document: ElementTree.Element, key: str) -> ElementTree.Element:
+        for element in document:
+            if key == self.get_attribute(element, "key"):
+                return element
+        raise KeyError("Key not found")
 
-    def template_modal(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
-        """This method is used to template a modal, by identifying it by its key and using the template engine to
-        template it.
+    def deserialize(self, source: str, key: K_contra, callables: Dict[str, Callback]) -> ReturnType:
+        """This method is used to deserialize the embed from the XML file.
 
         Args:
-            key (K): key of the modal
-            template_engine (TemplateEngine): template engine that is used to template the modal
-            keywords (Dict[str, Any]): keywords that are used to template the modal
+            source (str): raw string containing the element
+            key (K): key of the element
+            callables (Dict[str, Callback]): dictionary containing the callables to use for the components
 
-        Returns (str): templated modal
+        Returns (Message): message containing the embed and its view
         """
-        return template_engine.template(self.get_modal(key), keywords)
+        document = ElementTree.fromstring(source)
+        element = self._get_element(document, key)
+        return self.deserialize_element(document, element, callables)
 
+    def deserialize_element(
+            self,
+            document: ElementTree.Element,
+            element: ElementTree.Element,
+            callables: Dict[str, Callback]
+    ) -> ReturnType:
+        """This method is used to deserialize the embed from the XML file.
+
+        Args:
+            document (ElementTree.Element): document containing all the elements
+            element (ElementTree.Element): element containing the embed
+            callables (Dict[str, Callback]): dictionary containing the callables to use for the components
+
+        Returns (ReturnType): all possible deserialized objects.
+        """
+        element_type = ElementTypes.from_str(element.tag)
+
+        deserializers: Dict[ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], ReturnType]] = {
+            ElementTypes.MESSAGE: self.deserialize_message,
+            ElementTypes.EXPANSIVE: bind_menu(self.deserialize_expansive),
+            ElementTypes.MENU: bind_menu(partial(self.deserialize_menu, document=document)),
+            ElementTypes.MODAL: self.deserialize_modal,
+        }
+        assert element_type is not None, f"Element type {element.tag} not found"
+        return deserializers[element_type](element, callables)
 
-class XMLDeserializer(Deserializer):
-    """Read and process the data given by the XML file, and use given user objects to render the text"""
-
-    def deserialize_into_message(self, source: str, callables: Dict[str, Callback], **kw) -> Message:
+    def deserialize_expansive(self, element: ElementTree.Element, callbacks: Dict[str, Callback]) -> List[Message]:
         """Deserializes an embed from an XML file, and returns it as a Display object.
 
         Args:
-            source (str): templated document contents to deserialize.
-            callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            **kw (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
+            element (ElementTree.Element): templated document contents to deserialize.
+            callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the components.
 
         Returns (Display): A display object containing the embed and its view.
         """
-        return self.deserialize_message(ElementTree.fromstring(source), callables, kw)
+        raw_embed = element.find("embed")
+        assert raw_embed is not None, "Embed not found"
+        timeout_element = element.find("timeout")
+        timeout: Optional[float] = 180.0
+        if timeout_element is not None:
+            timeout = None if timeout_element.text is None else float(timeout_element.text)
+        messages = [self.deserialize_message(element, callbacks, embed=embed)
+                    for embed in self._separate_embed(raw_embed, element.get("page_number_key"))]
+        attach_views(messages, timeout)
+
+        return messages
 
     def deserialize_message(
             self,
             message_tree: ElementTree.Element,
             callables: Dict[str, Callback],
-            kwargs: Dict[str, Any],
+            **overrides: Any
     ) -> Message:
         """Deserializes an embed from an ElementTree.Element, and returns it as a Display object.
 
         Args:
             message_tree (ElementTree.Element): The element to deserialize the embed from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            kwargs (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
+            **overrides (Any): any overrides to apply to the Message
 
         Returns (Message): A display object containing the embed and its view.
         """
-
-        def get_text(element_tree: ElementTree.Element, child: str) -> Optional[str]:
-            element = element_tree.find(child)
-            if element is None:
-                return None
-            return None if element.text is None else element.text
-
-        def get_element(element_tree: ElementTree.Element, child: str) -> Optional[ElementTree.Element]:
-            return None if (element := element_tree.find(child)) is None else element
-
-        def apply(
-                element: Optional[M],
-                func: Callable[Concatenate[M, P], N],
-                *args: P.args,
-                **keyword_args: P.kwargs,
-        ) -> Optional[N]:
-            if element is None:
-                return None
-            return func(element, *args, **keyword_args)
-
-        return Message(
+        message = Message(
             embed=apply(get_element(message_tree, "embed"), self._render_embed),
             embeds=apply(
                 get_element(message_tree, "embeds"),
                 lambda raw_tree: list(map(self._render_embed, raw_tree)),
             ),
-            view=apply(get_element(message_tree, "view"), self._render_view, callables, kwargs),
+            view=apply(get_element(message_tree, "view"), self._render_view, callables),
             content=get_text(message_tree, "content"),
             tts=apply(get_text(message_tree, "tts"), lambda string: string.lower() == "true"),
             nonce=apply(get_text(message_tree, "nonce"), int),
             delete_after=apply(get_text(message_tree, "delete_after"), float),
             suppress_embeds=apply(
                 get_element(message_tree, "suppress_embeds"),
                 lambda tree: self.get_attribute(tree, "value") in ("", "true"),
@@ -206,63 +183,123 @@
                 lambda tree: self.get_attribute(tree, "value") in ("", "true"),
             ),
             stickers=None,
             ephemeral=None,
             silent=apply(
                 get_element(message_tree, "silent"),
                 lambda tree: self.get_attribute(tree, "value") in ("", "true"),
-            )
+            ),
         )
+        for key, value in overrides.items():
+            setattr(message, key, value)
+        return message
+
+    def deserialize_page(
+            self,
+            document: ElementTree.Element,
+            element: ElementTree.Element,
+            callables: Dict[str, Callback]
+    ) -> List[Message]:
+        if element.tag == "page":
+            element = self._get_element(document, self.get_attribute(element, "key"))
+        element_type = ElementTypes.from_str(element.tag)
+
+        def wrap_in_list(
+                method: Callable[[ElementTree.Element, Dict[str, Callback]], Message]
+        ) -> Callable[[ElementTree.Element, Dict[str, Callback]], List[Message]]:
+            def wrapper(page: ElementTree.Element, callback: Dict[str, Callback]) -> List[Message]:
+                return [method(page, callback)]
+
+            return wrapper
+
+        page_deserializers: Dict[
+            ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], List[Message]]] = {
+            ElementTypes.MESSAGE: wrap_in_list(self.deserialize_message),
+            ElementTypes.EXPANSIVE: self.deserialize_expansive,
+        }
+        assert element_type is not None, f"Element type {element.tag} not found"
+        return page_deserializers[element_type](element, callables)
 
-    def deserialize_into_menu(self, source: str, callables: Dict[str, Callback], **kw) -> List[Message]:
+    def deserialize_menu(
+            self,
+            element: ElementTree.Element,
+            callables: Dict[str, Callback],
+            *,
+            document: ElementTree.Element,
+    ) -> List[Message]:
         """Deserializes a menu from an XML file, by generating a list of displays that are connected by buttons in their
         views to navigate between them.
 
         Args:
-            source (str): The XML file to deserialize.
+            element (ElementTree.Element): The XML Menu Element to deserialize.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            **kw (Dict[str, Any]): A dictionary containing the keyword arguments to use for the views.
+            document (ElementTree.Element): The entire document
 
         Returns (List[Display]): List of displays that are connected by buttons in their views to navigate between them.
         """
+        raw_pages = element.find("pages")
+        assert raw_pages is not None, "pages is not present"
 
-        menu_tree: ElementTree.Element = ElementTree.fromstring(source)
-        return [self.deserialize_message(embed, callables, kw) for embed in menu_tree.findall("message")]
-
-    def deserialize_into_modal(self, source: str, methods: Dict[str, Callback], **kwargs: Any) -> discord.ui.Modal:
-        """Method to deserialize a modal into a discord.ui.Modal object
+        pages: List[Message] = sum([self.deserialize_page(document, page, callables) for page in raw_pages], [])
 
-        Args:
-            source (str): The source text to deserialize into a modal
-            methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            **kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
+        timeout = element.find("timeout")
+        attach_views(pages, float(timeout.text) if timeout is not None and timeout.text is not None else None)
 
-        Returns (discord.ui.Modal): A discord.ui.Modal object
-        """
-        modal_tree = ElementTree.fromstring(source)
-        return self._render_modal(modal_tree, methods, **kwargs)
+        return pages
 
-    def _render_modal(self, tree: ElementTree.Element, methods: Dict[str, Callback], **kwargs: Any) -> discord.ui.Modal:
-        """Method to render a modal from a modal tree
+    def deserialize_modal(
+            self,
+            element: ElementTree.Element,
+            methods: Dict[str, Callback],
+            **kwargs: Any
+    ) -> discord.ui.Modal:
+        """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
-            tree (Dict[str, Any]): The modal tree to render
+            element (ElementTree.Element): The element to deserialize into a modal
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
             kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
-        title = self.get_attribute(tree, "title")
+        title = self.get_attribute(element, "title")
         modal = type(f"{title} Modal", (discord.ui.Modal,), {**methods, **kwargs})(title=title)
 
-        for component in self.render_components(tree):
+        for component in self.render_components(element):
             modal.add_item(component)
 
         return modal
 
+    def _separate_embed(self, raw_embed: ElementTree.Element, replacement_key: Optional[str]) -> List[discord.Embed]:
+        """Separates the embeds from the raw embed element.
+
+        Args:
+            raw_embed (ElementTree.Element): The raw embed element.
+
+        Returns (List[discord.Embed]): A list of embeds.
+        """
+
+        def get(tree: ElementTree.Element, key: str) -> ElementTree.Element:
+            element = tree.find(key)
+            assert element is not None, f"{key} is not present"
+            return element
+
+        def get_element_text(tree: ElementTree.Element, key: str) -> str:
+            element_text = get(tree, key).text
+            assert element_text is not None, f"{key} is does not have text"
+            return element_text
+
+        expansive_text = get(raw_embed, "expansive_field")
+
+        return make_expansive_embeds(get_element_text(expansive_text, "name"),
+                                     get_element_text(expansive_text, "value"),
+                                     replacement_key,
+                                     raw_embed,
+                                     self._render_embed)
+
     @staticmethod
     def _render_reference(
             reference_tree: ElementTree.Element,
     ) -> discord.MessageReference:
         """Renders a message reference object from an ElementTree.Element.
 
         Args:
@@ -324,26 +361,29 @@
             description=self.get_element_text(raw_file.find("description")),
         )
 
     def _render_view(
             self,
             raw_view: ElementTree.Element,
             callables: Dict[str, Callback],
-            kwargs: Dict[str, Any],
     ) -> ui.View:
         """Renders a view from an ElementTree.Element.
 
         Args:
             raw_view (ElementTree.Element): The element to render the view from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            kwargs (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
 
         Returns (ui.View): A view object containing the components.
         """
-        view = ui.View(**kwargs)
+
+        view = ui.View()
+
+        timeout = raw_view.find("timeout")
+        if timeout is not None:
+            view.timeout = None if timeout.text is None else float(timeout.text)
         for component in self.render_components(raw_view, callables):
             view.add_item(component)
         return view
 
     @staticmethod
     def get_element_text(element: Optional[ElementTree.Element]) -> str:
         """Renders the given ElementTree.Element by returning its text.
@@ -415,17 +455,15 @@
         """Renders the fields from an ElementTree.Element.
 
         Args:
             fields_element (ElementTree.Element): The element to render the fields from.
 
         Returns (List[dict]): A list of dictionaries containing the raw fields.
         """
-        assert fields_element is not None, "Expected Fields For Embed"
-
-        return [
+        return [] if fields_element is None else [
             {
                 "name": self.get_element_text(field.find("name")),
                 "value": self.get_element_text(field.find("value")),
                 "inline": self.get_attribute(field, "inline").lower() == "true",
             }
             for field in fields_element.findall("field")
         ]
@@ -626,34 +664,41 @@
             callables (Dict[str, Callback]): The callbacks to use if the user interacts with the components.
 
         Returns (Optional[List[discord.ui.Item]]): The rendered components.
         """
         if callables is None:
             callables = {}
 
+        components = view.find("components")
+        if components is None:
+            return []
         return [
             self.render_component(
                 component,
                 callables.get(self.get_attribute(component, "key")),
             )
-            for component in view
+            for component in components
         ]
 
-    def _render_embed(self, raw_embed: ElementTree.Element) -> discord.Embed:
+    def _render_embed(self, raw_embed: ElementTree.Element, *replacements: Tuple[str, str]) -> discord.Embed:
         """Render the desired templated embed in discord.Embed instance.
 
         Args:
            raw_embed(ElementTree.Element): The element to render the embed from.
+           *replacements:
 
         Returns:
             Embed: Embed Object, discord compatible.
         """
 
-        def render(name: str):
-            return self.get_element_text(raw_embed.find(name))
+        def render(name: str) -> str:
+            element_text = self.get_element_text(raw_embed.find(name))
+            for replacement in replacements:
+                element_text = element_text.replace(*replacement)
+            return element_text
 
         embed_type: embed_types.EmbedType = "rich"
         if cast(embed_types.EmbedType, given_type := render("type")) != "":
             embed_type = cast(embed_types.EmbedType, given_type)
 
         embed = discord.Embed(
             title=render("title"),
```

### Comparing `discord-qalib-2.1.2/setup.py` & `discord-qalib-2.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.1.2",
+    version="2.2.0",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
+    package_data={"qalib": ["py.typed"]},
 )
```


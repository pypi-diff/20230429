# Comparing `tmp/discord-qalib-2.2.0.tar.gz` & `tmp/discord-qalib-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.2.0.tar", last modified: Sat Apr 29 18:14:18 2023, max compression
+gzip compressed data, was "discord-qalib-2.2.1.tar", last modified: Sat Apr 29 18:21:38 2023, max compression
```

## Comparing `discord-qalib-2.2.0.tar` & `discord-qalib-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 18:14:18.000000 discord-qalib-2.2.0/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 18:13:46.000000 discord-qalib-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:14:18.571757 discord-qalib-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-29 18:14:05.000000 discord-qalib-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.016867 discord-qalib-2.2.1/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/setup.py
```

### Comparing `discord-qalib-2.2.0/LICENSE` & `discord-qalib-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/PKG-INFO` & `discord-qalib-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.0
+Version: 2.2.1
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
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.0/README.md` & `discord-qalib-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.2.1/discord_qalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.0
+Version: 2.2.1
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
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.2.0/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.2.1/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/pyproject.toml` & `discord-qalib-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.2.0"
+version = "2.2.1"
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
-version = "2.2.0"
+version = "2.2.1"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.2.0/qalib/__init__.py` & `discord-qalib-2.2.1/qalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .template_engines.jinja2 import Jinja2
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.2.0/qalib/context.py` & `discord-qalib-2.2.1/qalib/context.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/interaction.py` & `discord-qalib-2.2.1/qalib/interaction.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/renderer.py` & `discord-qalib-2.2.1/qalib/renderer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/template_engines/formatter.py` & `discord-qalib-2.2.1/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/template_engines/jinja2.py` & `discord-qalib-2.2.1/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/__init__.py` & `discord-qalib-2.2.1/qalib/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/deserializer.py` & `discord-qalib-2.2.1/qalib/translators/deserializer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/factory.py` & `discord-qalib-2.2.1/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/json.py` & `discord-qalib-2.2.1/qalib/translators/json.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/message_parsing.py` & `discord-qalib-2.2.1/qalib/translators/message_parsing.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/templater.py` & `discord-qalib-2.2.1/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/qalib/translators/xml.py` & `discord-qalib-2.2.1/qalib/translators/xml.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.0/setup.py` & `discord-qalib-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.2.0",
+    version="2.2.1",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```


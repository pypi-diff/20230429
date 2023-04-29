# Comparing `tmp/PythonToolsKit-1.2.3.tar.gz` & `tmp/PythonToolsKit-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToolsKit-1.2.3.tar", last modified: Sun Apr  9 12:17:42 2023, max compression
+gzip compressed data, was "PythonToolsKit-1.2.4.tar", last modified: Sat Apr 29 07:51:18 2023, max compression
```

## Comparing `PythonToolsKit-1.2.3.tar` & `PythonToolsKit-1.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PythonToolsKit/
--rw-r--r--   0 kali      (1000) kali      (1000)    14047 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Arguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8544 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Characters.py
--rw-r--r--   0 kali      (1000) kali      (1000)    27309 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    43063 2023-04-09 12:17:05.000000 PythonToolsKit-1.2.3/PythonToolsKit/DataAnalysis.py
--rw-r--r--   0 kali      (1000) kali      (1000)    18433 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/DebugEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5865 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Dict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4454 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/DictObject.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11285 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Encodings.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2665 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Function.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3705 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetFile.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3814 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetPass.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19640 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetType.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2404 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Import.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5264 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Json.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3237 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/List.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8596 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Logs.py
--rw-r--r--   0 kali      (1000) kali      (1000)    16573 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/OrdDict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5353 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/PrintF.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3394 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Process.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6193 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Random.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2490 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/RecursionDebug.py
--rw-r--r--   0 kali      (1000) kali      (1000)    18332 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Report.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4888 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/ScapyTools.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7137 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/StringF.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15551 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Terminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/TestArguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4712 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/TestTimeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3098 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Thread.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7868 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Timeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3264 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Tuple.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10022 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/WindowsTerminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-04-09 12:16:27.000000 PythonToolsKit-1.2.3/PythonToolsKit/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5949 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/urlopen.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PythonToolsKit/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14031 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Arguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8577 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Characters.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    27267 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Colors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    42937 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DataAnalysis.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19183 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DebugEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5837 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Dict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4452 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DictObject.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11277 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Encodings.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2661 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Function.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3701 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetFile.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3810 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetPass.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19618 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetType.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2400 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5260 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Json.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3225 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/List.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8574 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Logs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16523 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/OrdDict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5351 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/PrintF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3392 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Process.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6189 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Random.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2488 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/RecursionDebug.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    18306 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Report.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9654 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/ScapyTools.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7131 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/StringF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15457 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Terminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/PythonToolsKit/TestArguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4710 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/TestTimeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Thread.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7854 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Timeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3252 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Tuple.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10004 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/WindowsTerminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-04-29 13:21:36.000000 PythonToolsKit-1.2.4/PythonToolsKit/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5935 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/urlopen.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/setup.py
```

### Comparing `PythonToolsKit-1.2.3/LICENSE.txt` & `PythonToolsKit-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.3/PKG-INFO` & `PythonToolsKit-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.3
+Version: 1.2.4
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Arguments.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
 global verbose
 verbose = lambda *x: None  # default do nothing (mode verbose not active)
 vprint = partial(print, "[V]")
 
 
 def set_verbose(verbose_function: Callable = vprint) -> None:
-
     """
     This function sets verbose mode.
     """
 
     global verbose
 
     module_caller_globals = stack()[
@@ -111,15 +110,14 @@
             if value is verbose:
                 module_caller_globals[key] = verbose_function
 
     verbose = verbose_function
 
 
 def set_debug() -> None:
-
     """
     This function sets log level for all loggers.
     """
 
     basicConfig(level=DEBUG)
     [getLogger(name).setLevel(DEBUG) for name in root.manager.loggerDict]
 
@@ -147,15 +145,14 @@
         prompt_function: Callable = getpass,
         prompt_function_args: List[Any] = [],
         prompt_function_kwargs: List[Any] = {},
         password_kwargs: Dict[str, Any] = {},
         prompt_kwargs: Dict[str, Any] = {},
         mutually_group_kwargs: Dict[str, Any] = {},
     ) -> Tuple[_MutuallyExclusiveGroup, _StoreAction, _StoreAction]:
-
         """
         This function add password argument and password prompt
         arguments.
         """
 
         # max_prompt = max(prompt_args, key=lambda x: len(x))
         # for arg in prompt_args:
@@ -191,15 +188,14 @@
     def add_input_file(
         self,
         *args,
         file_args: List[Any] = [],
         file_kwargs: Dict[str, Any] = {},
         **kwargs,
     ) -> _StoreAction:
-
         """
         This function add input file argument.
 
         By default if not present in the command line
         the value is None. If is present in the command line
         but no value follow use the stdin. If present with a
         value, the ArgumentParser will try to open the file.
@@ -226,15 +222,14 @@
     def add_output_file(
         self,
         *args,
         file_args: List[Any] = ["w"],
         file_kwargs: Dict[str, Any] = {},
         **kwargs,
     ) -> _StoreAction:
-
         """
         This function add output file argument.
 
         By default if not present in the command line
         the value is stdout. If is present in the command line
         but no value follow use the stdout. If present with a
         value, the ArgumentParser will try to open the file.
@@ -261,15 +256,14 @@
         kwargs2.update(kwargs)
 
         return self.add_argument(*args, **kwargs2)
 
     def add_verbose(
         self, *args, function: Callable = vprint, **kwargs
     ) -> _StoreAction:
-
         """
         This method adds verbose argument to the parser.
         """
 
         if not args:
             args = ["--verbose", "-v"]
 
@@ -284,15 +278,14 @@
         argument = self.add_argument(*args, **default_kwargs)
         self.verbose_destination = argument.dest
         self.verbose_function = function
 
         return argument
 
     def add_debug(self, *args, **kwargs) -> _StoreAction:
-
         """
         This method adds debug argument to the parser.
         """
 
         if not args:
             args = ["--debug", "-d"]
 
@@ -306,15 +299,14 @@
 
         argument = self.add_argument(*args, **default_kwargs)
         self.debug_destination = argument.dest
 
         return argument
 
     def parse_args(self, *args, **kwargs) -> Namespace:
-
         """
         This function parse command line arguments.
         """
 
         response = _ArgumentParser.parse_args(self, *args, **kwargs)
 
         password_prompt_destination = self.password_prompt_destination
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Characters.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,83 +109,83 @@
     >>> str(chars)
     'TEXT: abc\\nINT: 97 98 99\\nHEXA: 61 62 63\\nBINARY: 01100001 01100010 01100011'
     >>> print(chars)
     TEXT: abc
     INT: 97 98 99
     HEXA: 61 62 63
     BINARY: 01100001 01100010 01100011
-    >>> 
+    >>>
     """
 
     def __init__(self):
         self.hexa: str = None
         self.string: str = None
         self.bin: List[str] = None
         self.int: List[int] = None
-        self.translate = str.maketrans('', '', ': -')
+        self.translate = str.maketrans("", "", ": -")
 
     def __str__(self) -> str:
         return (
             f"TEXT: {self.text}\nINT: {' '.join([str(x) for x in self.int])}"
             f"\nHEXA: {self.hexa}\nBINARY: {' '.join(self.bin)}"
         )
-        
+
     def __repr__(self) -> str:
         return self.__class__.__name__ + "(" + self.__str__() + ")"
 
     def from_string(self, data: str) -> Tuple[str, List[int], str, List[str]]:
-
         """
         This method returns integers, hexadecimal and binary from string.
 
         >>> chars = Characters()
         >>> chars.from_string("abc")
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
-        >>> 
+        >>>
         """
 
         text = self.text = data
         integers = self.int = [ord(car) for car in data]
         hexa = self.hexa = hexlify(data.encode("latin"), " ").decode()
         binary = self.bin = [f"{integer:0>8b}" for integer in integers]
 
         return text, integers, hexa, binary
 
-    def from_int(self, data: List[int]) -> Tuple[str, List[int], str, List[str]]:
-
+    def from_int(
+        self, data: List[int]
+    ) -> Tuple[str, List[int], str, List[str]]:
         """
         This method returns string, hexadecimal and binary from integers.
 
         >>> chars = Characters()
         >>> chars.from_int([97, 98, 99])
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
-        >>> 
+        >>>
         """
 
         integers = self.int = data
         text = self.text = bytes(data).decode("latin1")
         hexa = self.hexa = hexlify(self.text.encode("latin"), " ").decode()
         binary = self.bin = [f"{integer:0>8b}" for integer in integers]
 
         return text, integers, hexa, binary
 
-    def from_bytes(self, encoded: bytes) -> Tuple[str, List[int], str, List[str]]:
-
+    def from_bytes(
+        self, encoded: bytes
+    ) -> Tuple[str, List[int], str, List[str]]:
         """
         This method returns string, hexadecimal, integers and binary from bytes.
 
         >>> chars = Characters()
         >>> chars.from_bytes(b'abc')
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
         """
 
         return self.from_int([x for x in encoded])
 
     def from_hexa(self, hexa: str) -> Tuple[str, List[int], str, List[str]]:
-
         """
         This method returns string, integers and binary from hexadecimal.
          - formats accepted: "a1 b4 ff", "A1B4FF" and "A1-b4-Ff"
 
         >>> chars = Characters()
         >>> chars.from_hexa('61 62 63')
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
@@ -193,29 +193,30 @@
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
         >>> chars.from_hexa('61-62-63')
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
         >>> chars.from_hexa('616263')
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
         >>> chars.from_hexa("5e 6F4f")
         ('^oO', [94, 111, 79], '5e 6f 4f', ['01011110', '01101111', '01001111'])
-        >>> 
+        >>>
         """
 
-        return self.from_bytes(b16decode(hexa.translate(self.translate).upper().encode()))
+        return self.from_bytes(
+            b16decode(hexa.translate(self.translate).upper().encode())
+        )
 
     def from_bin(self, binary: str) -> Tuple[str, List[int], str, List[str]]:
-
         """
         This method returns string, hexadecimal, and integers from binary.
          - format accepted: "1100001 1100010 1100011"
 
         >>> chars = Characters()
         >>> chars.from_bin('01100001 01100010 01100011')
         ('abc', [97, 98, 99], '61 62 63', ['01100001', '01100010', '01100011'])
-        >>> 
+        >>>
         """
 
         return self.from_int([int(x, 2) for x in binary.split()])
 
 
 def main() -> int:
     help_message = f"""USAGE: {executable} {argv[0]} [OPTION] ascii
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Colors.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 class Colors:
 
     """
     This class implements functions to translate colors.
     """
 
     def check_int_to_html(*args) -> str:
-
         """
         This function performs checks for int_to_html
         arguments and call it.
 
         >>> Colors.check_int_to_html(255, 0, 150)
         '#ff0096'
         >>> Colors.check_int_to_html(256, -1, "invalid")
@@ -151,15 +150,14 @@
                     "Colors.int_to_html arguments should "
                     f"be int between 0 and 255 ({arg!r} is invalid)."
                 )
 
         return Colors.int_to_html(*args)
 
     def safe_int_to_html(*args) -> str:
-
         """
         This function performs checks for int_to_html
         arguments and call it.
 
         >>> Colors.safe_int_to_html(255, 0, 150)
         '#ff0096'
         >>> Colors.safe_int_to_html(256, -1, "invalid")
@@ -176,27 +174,25 @@
                 arg = arg % 256
 
             append(arg)
 
         return Colors.int_to_html(*args_)
 
     def int_to_html(red: int, green: int, blue: int) -> str:
-
         """
         This function translates integers colors to HTML colors.
 
         >>> Colors.int_to_html(255, 0, 150)
         '#ff0096'
         >>>
         """
 
         return "#" + b2a_hex(bytes((red, green, blue))).decode()
 
     def check_html_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for html_to_int
         arguments and call it.
 
         >>> Colors.check_html_to_int('#FF0096')
         (255, 0, 150)
         >>> Colors.check_html_to_int(7)
@@ -229,15 +225,14 @@
                 "string of length 7 starting with"
                 f" '#' ({color!r} is invalid)."
             )
 
         return Colors.html_to_int(color)
 
     def safe_html_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for html_to_int
         arguments and call it.
 
         >>> Colors.safe_html_to_int('#FF0096')
         (255, 0, 150)
         >>> Colors.safe_html_to_int('!FF0Z')
@@ -255,29 +250,27 @@
 
         while len(color_) < 7:
             color_ += "0"
 
         return Colors.html_to_int(color_)
 
     def html_to_int(colors: str) -> Tuple[int, int, int]:
-
         """
         This function translates HTML colors to integers colors.
 
         >>> Colors.html_to_int('#FF0096')
         (255, 0, 150)
         >>> Colors.html_to_int('#ff0096')
         (255, 0, 150)
         >>>
         """
 
         return tuple(x for x in a2b_hex(colors[1:].encode()))
 
     def check_rgb_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for rgb_to_int
         arguments and call it.
 
         >>> Colors.check_rgb_to_int('rgb(255, 0, 150)')
         (255, 0, 150)
         >>> Colors.check_rgb_to_int('rgb ( 255 , 0 , 150 ) ')
@@ -337,15 +330,14 @@
                 "three byte values separated by commas (example:"
                 f" 'rgb(255, 0, 2)') ({color!r} is invalid)."
             )
 
         return Colors.rgb_to_int(color)
 
     def safe_rgb_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for rgb_to_int
         arguments and call it.
 
         >>> Colors.safe_rgb_to_int('rgb(255, 0, 150)')
         (255, 0, 150)
         >>> Colors.safe_rgb_to_int('rgb(255, 0, 150,)')
@@ -377,28 +369,26 @@
         while counter < 3:
             color_ += "0, "
             counter += 1
 
         return Colors.rgb_to_int(color_[:-2] + ")")
 
     def rgb_to_int(colors: str) -> Tuple[int, int, int]:
-
         """
         This function translates RGB (CSS function)
         colors to integers colors.
 
         >>> Colors.rgb_to_int('rgb(255, 0, 150)')
         (255, 0, 150)
         >>>
         """
 
         return tuple(int(x) for x in colors.strip("rgb() ").split(","))
 
     def check_rgba_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for rgba_to_int
         arguments and call it.
 
         >>> Colors.check_rgba_to_int('rgba(255, 0, 150, 0.0)')
         (255, 0, 150)
         >>> Colors.rgba_to_int('rgba ( 255 , 0 , 150 , 1) ')
@@ -470,15 +460,14 @@
                 "three byte values separated by commas and a float between 0 and 1"
                 f" (example: 'rgba(255, 0, 2, 0.5)') ({color!r} is invalid)."
             )
 
         return Colors.rgba_to_int(color)
 
     def safe_rgba_to_int(color: str) -> Tuple[int, int, int]:
-
         """
         This function performs checks for rgba_to_int
         arguments and call it.
 
         >>> Colors.safe_rgba_to_int('rgba(255, 0, 150, 0.5)')
         (255, 0, 150)
         >>> Colors.safe_rgba_to_int('rgba(0.5)')
@@ -510,28 +499,26 @@
         while counter < 3:
             color_ += "0, "
             counter += 1
 
         return Colors.rgba_to_int(color_ + "0.5)")
 
     def rgba_to_int(colors: str) -> Tuple[int, int, int]:
-
         """
         This function translates RGBA (CSS function)
         colors to integers colors.
 
         >>> Colors.rgba_to_int('rgba(255, 0, 150, 0.5)')
         (255, 0, 150)
         >>>
         """
 
         return tuple(int(x) for x in colors.strip("rgba() ").split(",")[:3])
 
     def check_int_to_rgba(*args) -> str:
-
         """
         This function performs checks for int_to_rgba
         arguments and call it.
 
         >>> Colors.check_int_to_rgba(255, 0, 150, 0.5)
         'rgba(255, 0, 150, 0.5)'
         >>> Colors.check_int_to_rgba(256, -1, "invalid")
@@ -567,15 +554,14 @@
                 "Colors.int_to_rgba arguments should "
                 f"be int between 0 and 255 ({arg!r} is invalid)."
             )
 
         return Colors.int_to_rgba(*args[:4])
 
     def safe_int_to_rgba(*args) -> str:
-
         """
         This function performs checks for int_to_rgba
         arguments and call it.
 
         >>> Colors.safe_int_to_rgba(255, 0, 150)
         'rgba(255, 0, 150, 1)'
         >>> Colors.safe_int_to_rgba(256, -1, "invalid", 1.9)
@@ -605,28 +591,26 @@
                 )
 
         return Colors.int_to_rgba(*args_)
 
     def int_to_rgba(
         red: int, green: int, blue: int, transparency: float = 1
     ) -> str:
-
         """
         This function translates integers
         colors to RGBA (CSS function) colors.
 
         >>> Colors.int_to_rgba(255, 0, 150)
         'rgba(255, 0, 150, 1)'
         >>>
         """
 
         return f"rgba({red}, {green}, {blue}, {transparency})"
 
     def check_int_to_rgb(*args) -> str:
-
         """
         This function performs checks for int_to_rgb
         arguments and call it.
 
         >>> Colors.check_int_to_rgb(255, 0, 150)
         'rgb(255, 0, 150)'
         >>> Colors.check_int_to_rgb(256, -1, "invalid")
@@ -650,15 +634,14 @@
                     "Colors.int_to_rgb arguments should "
                     f"be int between 0 and 255 ({arg!r} is invalid)."
                 )
 
         return Colors.int_to_rgb(*args)
 
     def safe_int_to_rgb(*args) -> str:
-
         """
         This function performs checks for int_to_rgb
         arguments and call it.
 
         >>> Colors.safe_int_to_rgb(255, 0, 150)
         'rgb(255, 0, 150)'
         >>> Colors.safe_int_to_rgb(256, -1, "invalid")
@@ -675,28 +658,26 @@
                 arg = arg % 256
 
             append(arg)
 
         return Colors.int_to_rgb(*args_)
 
     def int_to_rgb(red: int, green: int, blue: int) -> str:
-
         """
         This function translates integers
         colors to RGB (CSS function) colors.
 
         >>> Colors.int_to_rgb(255, 0, 150)
         'rgb(255, 0, 150)'
         >>>
         """
 
         return f"rgb({red}, {green}, {blue})"
 
     def check_get_8bits_color(*args) -> int:
-
         """
         This function performs checks for get_8bits_color
         arguments and call it.
 
         >>> Colors.check_get_8bits_color(7, 7, 3)
         255
         >>> Colors.check_get_8bits_color(255, -1, "invalid")
@@ -727,15 +708,14 @@
                     "be int between 0 and 7 and the third should be int "
                     f"between 0 and 4 ({arg!r} is invalid)."
                 )
 
         return Colors.get_8bits_color(*args)
 
     def safe_get_8bits_color(*args) -> int:
-
         """
         This function performs checks for get_8bits_color
         arguments and call it.
 
         >>> Colors.safe_get_8bits_color(7, 7, 3)
         255
         >>> Colors.safe_get_8bits_color(255, 150, "abc")
@@ -756,15 +736,14 @@
 
             counter += 1
             append(arg)
 
         return Colors.get_8bits_color(*args_)
 
     def get_8bits_color(red: int, green: int, blue: int) -> int:
-
         """
         This function returns integer (0-255) representing 8bits-1byte colors.
 
         >>> Colors.get_8bits_color(7, 7, 3)
         255
         >>> Colors.get_8bits_color(0, 0, 0)
         0
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/DataAnalysis.py` & `PythonToolsKit-1.2.4/PythonToolsKit/DataAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,15 +397,14 @@
     PYPLOT = True
 
 Value = TypeVar("Value", str, int, float, complex, datetime, None)
 DataAnalysis = TypeVar("DataAnalysis")
 
 
 class DataAnalysis:
-
     valuetype = namedtuple("valuetype", ["key", "value", "counter"])
     statistictype = namedtuple("statistictype", ["key", "value"])
 
     def __init__(
         self,
         data: Iterable[Union[Dict[Hashable, Value]], Iterable[Value]],
         fields: List[Hashable] = None,
@@ -420,26 +419,24 @@
         self.keys = defaultdict(lambda: defaultdict(int))
         self.build_keys()
 
     @staticmethod
     def get_iterator_tuples(
         data: Iterable[Union[Dict[Hashable, Value]], Iterable[Value]]
     ) -> Iterable[Tuple[Hashable, Value]]:
-
         """
         This function returns an iterator of tuples from dict or Iterable.
         """
 
         if isinstance(data, dict):
             return data.items()
         else:
             return enumerate(data)
 
     def build_keys(self) -> None:
-
         """
         This function build data keys (reqired for all functions).
         """
 
         keys = self.keys
         fields = self.fields
         filters = self.filters
@@ -448,155 +445,139 @@
 
         get_iterator_tuples = self.get_iterator_tuples
         filters_get = filters.get
 
         for data in datas:
             elements = get_iterator_tuples(data)
             for key, value in elements:
-
                 filter_ = filters_get(key)
                 if (fields_is_not_None and key not in fields) or (
                     filter_ and not filter_(value)
                 ):
                     continue
 
                 keys[key][value] += 1
 
     def get_numbers_by_key(
         self, key: Hashable
     ) -> Union[List[Union[int, float]], None]:
-
         """
         This function returns a list of numbers by key value.
         """
 
         all_values = []
         for value, counter in self.keys[key].items():
             if isinstance(value, (int, float)):
                 all_values.extend([value] * counter)
 
         return all_values or None
 
     def get_median(self, key: Hashable) -> statistictype:
-
         """
         This function returns median for a specific key.
         """
 
         return self.get_statistic(key, median)
 
     def get_medians(self) -> Iterable[statistictype]:
-
         """
         This function returns medians.
         """
 
         yield from self.get_statistics(median)
 
     def get_deviation(self, key: Hashable) -> statistictype:
-
         """
         This function returns deviation for a specific key.
         """
 
         return self.get_statistic(key, pstdev)
 
     def get_deviations(self) -> Iterable[statistictype]:
-
         """
         This function returns deviations.
         """
 
         yield from self.get_statistics(pstdev)
 
     def get_variance(self, key: Hashable) -> statistictype:
-
         """
         This function returns variance for a specific key.
         """
 
         return self.get_statistic(key, variance)
 
     def get_variances(self) -> Iterable[statistictype]:
-
         """
         This function returns variances.
         """
 
         yield from self.get_statistics(variance)
 
     def get_average(self, key: Hashable) -> statistictype:
-
         """
         This function returns average for a specific key.
         """
 
         return self.get_statistic(key, fmean)
 
     def get_averages(self) -> Iterable[statistictype]:
-
         """
         This function returns averages.
         """
 
         yield from self.get_statistics(fmean)
 
     def get_sum(self, key: Hashable) -> statistictype:
-
         """
         This function returns sum for a specific key.
         """
 
         return self.get_statistic(key, sum)
 
     def get_sums(self) -> Iterable[statistictype]:
-
         """
         This function returns sums.
         """
 
         yield from self.get_statistics(sum)
 
     def get_maximum(self, key: Hashable) -> statistictype:
-
         """
         This function returns maximum for a specific key.
         """
 
         return self.get_statistic(
             key,
             partial(max, key=lambda x: x.value),
             valuegetter=self.get_values_by_key,
         )
 
     def get_maximums(self) -> Iterable[statistictype]:
-
         """
         This function returns maximums.
         """
 
         yield from self.get_statistics(
             partial(max, key=lambda x: x.value),
             valuegetter=self.get_values_by_key,
         )
 
     def get_minimum(self, key: Hashable) -> statistictype:
-
         """
         This function returns minimum for a specific key.
         """
 
         return self.get_statistic(
             key,
             partial(min, key=lambda x: x.value),
             valuegetter=self.get_values_by_key,
         )
 
     def get_minimums(self) -> Iterable[statistictype]:
-
         """
         This function returns minimums.
         """
 
         yield from self.get_statistics(
             partial(min, key=lambda x: x.value),
             valuegetter=self.get_values_by_key,
@@ -604,15 +585,14 @@
 
     def get_statistic(
         self,
         key: Hashable,
         function: Callable,
         valuegetter: Callable = None,
     ) -> statistictype:
-
         """
         This function returns specific statistic for a specific key.
         """
 
         data = (
             valuegetter(key) if valuegetter else self.get_numbers_by_key(key)
         )
@@ -621,54 +601,50 @@
             if data
             else self.statistictype(key=key, value=data)
         )
 
     def get_statistics(
         self, function: Callable, valuegetter: Callable = None
     ) -> Iterable[statistictype]:
-
         """
         This function returns specific statistics.
         """
 
         get_statistic = self.get_statistic
         yield from (
             get_statistic(key, function, valuegetter)
             for key in self.keys.keys()
         )
 
     def count_value(self, key: Hashable, value: Value) -> valuetype:
-
         """
         This function returns valuetype representing
         a key value and counter of this value.
         """
 
         return self.valuetype(
             key=key, value=value, counter=self.keys[key][value]
         )
 
     def compare_values(
         self, function: Callable, value1: valuetype, value2: valuetype
     ) -> bool:
-
         """
         This function compares valuetypes.
         """
 
         return function(value1.value, value2.value)
 
     def compare_event_action(
         self,
         ref_value: valuetype,
         event: Callable,
         match_action: Callable,
         not_match_action: Callable = lambda x: None,
     ) -> Any:
-
         """
         This function calls match_action if event
         return is True else calls not_match_action.
 
         event signature: event(tested_value: valuetype, ref_value: valuetype) -> bool
         match_action signature: match_action(value: valuetype) -> Any
         not_match_action signature: not_match_action(value: valuetype) -> Any
@@ -678,184 +654,170 @@
             match_action(tested_value)
             if event(tested_value, ref_value)
             else not_match_action(tested_value)
             for tested_value in self.get_values()
         )
 
     def count_gt(self, value: valuetype) -> int:
-
         """
         This function counts values greater than value.
         """
 
         return sum(
             self.compare_event_action(
                 value,
                 partial(self.compare_values, gt),
                 lambda x: x.counter,
                 lambda x: 0,
             )
         )
 
     def count_lt(self, value: valuetype) -> int:
-
         """
         This function counts values lesser than value.
         """
 
         return sum(
             self.compare_event_action(
                 value,
                 partial(self.compare_values, lt),
                 lambda x: x.counter,
                 lambda x: 0,
             )
         )
 
     def get_gt(self, value: valuetype) -> Iterable[valuetype]:
-
         """
         This function yields valuetype greater than value.
         """
 
         yield from (
             self.compare_event_action(
                 value, partial(self.compare_values, gt), lambda x: x
             )
         )
 
     def get_lt(self, value: valuetype) -> Iterable[valuetype]:
-
         """
         This function yields valuetype lesser than value.
         """
 
         yield from (
             self.compare_event_action(
                 value, partial(self.compare_values, lt), lambda x: x
             )
         )
 
     def get_values_by_key(self, key: Hashable) -> Iterable[valuetype]:
-
         """
         This function returns the list of
         keys, values and counters for a key.
         """
 
         valuetype = self.valuetype
         yield from (
             valuetype(key=key, value=value, counter=counter)
             for value, counter in self.keys[key].items()
         )
 
     def count_values_by_key(self, key: Hashable) -> statistictype:
-
         """
         This functions returns a statistictype with
         key and counter of differents values for this key.
         """
 
         return self.statistictype(key=key, value=len(self.keys[key]))
 
     def count_values_by_keys(self) -> Iterable[statistictype]:
-
         """
         This functions returns statistictypes with
         key and counter of differents values for this key.
         """
 
         yield from (self.count_values_by_key(key) for key in self.keys.keys())
 
     def get_values(self) -> Iterable[valuetype]:
-
         """
         This function returns a list of
         each keys, values and counters.
         """
 
         valuetype = self.valuetype
         yield from (
             valuetype(key=key, value=value, counter=counter)
             for key, values in self.keys.items()
             for value, counter in values.items()
         )
 
     def get_all_values(self) -> Iterable[valuetype]:
-
         """
         This function returns a list of
         all keys, values and counters.
         """
 
         valuetype = self.valuetype
         yield from (
             valuetype(key=key, value=value, counter=counter)
             for key, values in self.keys.items()
             for value, counter in values.items()
             for x in range(counter)
         )
 
     def sort_by_value(self, *args, **kwargs) -> valuetype:
-
         """
         This functions returns keys, values
         and counters sorted by values.
         """
 
         return sorted(
             self.get_values(), *args, key=lambda x: x.value, **kwargs
         )
 
     def sort_values_by_sum(self, *args, **kwargs) -> Iterable[valuetype]:
-
         """
         This functions returns keys, values
         and counters sorted by sum of values.
         """
 
         return sorted(
             self.get_values(),
             *args,
             key=lambda x: x.value * x.counter,
             **kwargs,
         )
 
     def get_keys_counter(self) -> Counter:
-
         """
         This function returns a Counter object
         representing key and sum of the values.
         """
 
         counter = Counter()
 
         for key, values in self.keys.items():
             for value, number in values.items():
                 counter[key] += value * number
 
         return counter
 
     def get_values_counter(self) -> Counter:
-
         """
         This function returns a Counter object
         representing values and values count.
         """
 
         counter = Counter()
 
         for key, values in self.keys.items():
             for value, number in values.items():
                 counter[value] += number
 
         return counter
 
     def get_keys_values_counter(self) -> Counter:
-
         """
         This function returns a Counter object
         representing valuetypes and sum of the values.
         """
 
         counter = Counter()
         valuetype = self.valuetype
@@ -865,15 +827,14 @@
                 counter[valuetype(key=key, value=value, counter=number)] += (
                     value * number
                 )
 
         return counter
 
     def get_keys_values_count_counter(self) -> Counter:
-
         """
         This function returns a Counter object
         representing valuetypes and values count.
         """
 
         counter = Counter()
         valuetype = self.valuetype
@@ -885,82 +846,75 @@
                 ] += number
 
         return counter
 
     def sort_keys_by_sum(
         self, counter: Counter = None
     ) -> List[Tuple[Hashable, Value]]:
-
         """
         This functions returns keys and
         values sorted by sum of values.
         """
 
         counter = counter or self.get_keys_counter()
         return counter.most_common()
 
     def sort_by_counter(self, *args, **kwargs) -> Iterable[valuetype]:
-
         """
         This functions returns keys, values
         and counters sorted by counters.
         """
 
         return sorted(
             self.get_values(), *args, key=lambda x: x.counter, **kwargs
         )
 
     def sort_by_key(self, *args, **kwargs) -> Iterable[valuetype]:
-
         """
         This functions returns keys, values and counters sorted by counters.
         """
 
         return sorted(self.get_values(), *args, key=lambda x: x.key, **kwargs)
 
     @staticmethod
     def sort_dict_by_value(
         data: Dict[Hashable, Value], *args, **kwargs
     ) -> Dict[Hashable, Value]:
-
         """
         This functions returns the dict sorted by values.
         """
 
         return sorted(data, *args, key=lambda x: data[x], **kwargs)
 
     @staticmethod
     def sort_statistictype_by_value(
         data: Iterable[statistictype], *args, **kwargs
     ) -> Iterable[statistictype]:
-
         """
         This functions returns statistictypes sorted by values.
         """
 
         return sorted(data, *args, key=lambda x: x.value, **kwargs)
 
     @staticmethod
     def sort_statistictype_by_key(
         data: Iterable[statistictype], *args, **kwargs
     ) -> Iterable[statistictype]:
-
         """
         This functions returns statistictypes sorted by keys.
         """
 
         return sorted(data, *args, key=lambda x: x.key, **kwargs)
 
     @staticmethod
     def frequence(
         all_sum: Union[int, float],
         sample_sum: Union[int, float],
         pourcent: bool = True,
     ) -> Union[int, float]:
-
         """
         This function returns the frequence of sample in all.
         """
 
         return (
             (sample_sum / all_sum * 100)
             if pourcent
@@ -970,15 +924,14 @@
     def key_frequence(
         self,
         key: Hashable,
         pourcent: bool = True,
         counter: Counter = None,
         all_sum: Union[int, float] = None,
     ) -> statistictype:
-
         """
         This functions returns a statistictype of key frequence.
         """
 
         counter = counter or self.get_keys_counter()
         return self.statistictype(
             key=key,
@@ -986,15 +939,14 @@
                 all_sum or sum(counter.values()), counter[key], pourcent
             ),
         )
 
     def keys_frequences(
         self, pourcent: bool = True, counter: Counter = None
     ) -> Iterable[statistictype]:
-
         """
         This generator yields statistictypes of keys frequences.
         """
 
         counter = counter or self.get_keys_counter()
         all_sum = sum(counter.values())
         yield from (
@@ -1005,15 +957,14 @@
     def key_value_frequence(
         self,
         value: valuetype,
         pourcent: bool = True,
         counter: Counter = None,
         all_sum: Union[int, float] = None,
     ) -> statistictype:
-
         """
         This function returns a statistictype of
         the frequency of the sum of the values in
         the key.
         """
 
         counter = counter or self.get_keys_values_counter()
@@ -1023,15 +974,14 @@
                 all_sum or sum(counter.values()), counter[value], pourcent
             ),
         )
 
     def keys_values_frequences(
         self, pourcent: bool = True, counter: Counter = None
     ) -> Iterable[statistictype]:
-
         """
         This generator yields statistictypes of
         the frequency of the sum of the values in
         the key.
         """
 
         counter = counter or self.get_keys_values_counter()
@@ -1044,15 +994,14 @@
     def key_value_count_frequence(
         self,
         value: valuetype,
         pourcent: bool = True,
         counter: Counter = None,
         all_sum: Union[int, float] = None,
     ) -> statistictype:
-
         """
         This function returns a statistictype of
         the frequency of the sum of the values in
         the key.
         """
 
         counter = counter or self.get_keys_values_count_counter()
@@ -1062,15 +1011,14 @@
                 all_sum or sum(counter.values()), counter[value], pourcent
             ),
         )
 
     def keys_values_count_frequences(
         self, pourcent: bool = True, counter: Counter = None
     ) -> Iterable[statistictype]:
-
         """
         This generator yields statistictypes of
         the frequency of the sum of the values in
         the key.
         """
 
         counter = counter or self.get_keys_values_count_counter()
@@ -1083,15 +1031,14 @@
     def value_frequence(
         self,
         value: Value,
         pourcent: bool = True,
         counter: Counter = None,
         all_sum: Union[int, float] = None,
     ) -> statistictype:
-
         """
         This functions returns a statistictype of value frequence.
         """
 
         counter = counter or self.get_values_counter()
         return self.statistictype(
             key=value,
@@ -1099,15 +1046,14 @@
                 all_sum or sum(counter.values()), counter[value], pourcent
             ),
         )
 
     def values_frequences(
         self, pourcent: bool = True, counter: Counter = None
     ) -> Iterable[statistictype]:
-
         """
         This generator yields statistictypes of values frequences.
         """
 
         counter = counter or self.get_values_counter()
         all_sum = sum(counter.values())
         yield from (
@@ -1119,15 +1065,14 @@
     def get_grouped_DataAnalysis(
         cls: type,
         data: Iterable[Union[Dict[Hashable, Value]], Iterable[Value]],
         columns: Tuple[Hashable],
         *args,
         **kwargs,
     ) -> Iterable[DataAnalysis]:
-
         """
         This function returns a DataAnalysis instance
         for each group formatted by columns values.
         """
 
         groups = defaultdict(list)
         for key, element in cls.get_iterator_tuples(data):
@@ -1135,26 +1080,24 @@
                 element
             )
 
         yield from (cls(x, *args, **kwargs) for x in groups.values())
 
     @staticmethod
     def statistictypes_printer(data: Iterable[statistictype]) -> None:
-
         """
         This function prints statistictypes.
         """
 
         DataAnalysis.print_data(
             data, {0: "key                    ", 1: "value              "}
         )
 
     @staticmethod
     def valuetypes_printer(data: Iterable[valuetype]) -> None:
-
         """
         This function prints valuetypes.
         """
 
         DataAnalysis.print_data(
             data,
             {
@@ -1166,28 +1109,26 @@
 
     @staticmethod
     def print_data(
         data: Iterable[Union[Dict[Hashable, Value]], Iterable[Value]],
         headers: Dict[Hashable, Union[str, int]] = {},
         onetime: bool = False,
     ) -> None:
-
         """
         This function prints data.
 
         The headers are printed on the first
         row and set the width of the columns.
         """
 
         get_iterator_tuples = DataAnalysis.get_iterator_tuples
 
         def get_row(
             element: Dict[Hashable, Value], is_key: bool = False
         ) -> str:
-
             """
             This function format an element to be printed.
             """
 
             values = []
             append = values.append
             get = headers.get
@@ -1235,15 +1176,14 @@
     def statistictypes_chart(
         data: Iterable[statistictype],
         chart_title: str = "Statistictypes chart",
         *args,
         color=None,
         **kwargs,
     ) -> None:
-
         """
         This function shows a matplotlib chart of statistictypes.
         """
 
         keys = []
         values = []
         keys_append = keys.append
@@ -1260,15 +1200,14 @@
     def valuetypes_values_chart(
         data: Iterable[valuetype],
         chart_title: str = "Valuetypes (values) chart",
         *args,
         color=None,
         **kwargs,
     ) -> None:
-
         """
         This function shows a matplotlib chart of valuetypes.
         """
 
         DataAnalysis.statistictypes_chart(
             data, chart_title, *args, color=color, **kwargs
         )
@@ -1277,15 +1216,14 @@
     def valuetypes_counters_chart(
         data: Iterable[valuetype],
         chart_title: str = "Valuetypes (counters) chart",
         *args,
         color=None,
         **kwargs,
     ) -> None:
-
         """
         This function shows a matplotlib chart of statistictypes.
         """
 
         keys = []
         values = []
         keys_append = keys.append
@@ -1303,15 +1241,14 @@
         values: Iterable,
         keys: Iterable,
         chart_title: str = "DataAnalysis chart",
         *args,
         color=None,
         **kwargs,
     ) -> None:
-
         """
         This function shows a matplotlib chart.
         """
 
         if not color:
             min_value = min(values)
             max_value = max(values)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/DebugEncoding.py` & `PythonToolsKit-1.2.4/PythonToolsKit/DebugEncoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,101 +412,160 @@
 from typing import Dict, List, Tuple
 from collections import defaultdict
 from dataclasses import dataclass
 from contextlib import suppress
 from sys import exit, stdout
 from json import dump
 
+
 @dataclass
 class WorkingEncoding:
 
     """
     This dataclass stores working encodings (encode
-    and decode without raised exceptions) data. 
+    and decode without raised exceptions) data.
     """
 
     encoding: str
     decoding: str
     decoded_values: str
     bad_values: str
 
-def debug_encoding(values_to_test: str, bad_values: str = None, encoding: str = None, decoding: str = None) -> Tuple[List[WorkingEncoding], Dict[str, List[WorkingEncoding]]]:
 
+def debug_encoding(
+    values_to_test: str,
+    bad_values: str = None,
+    encoding: str = None,
+    decoding: str = None,
+) -> Tuple[List[WorkingEncoding], Dict[str, List[WorkingEncoding]]]:
     """
     This function helps developers to debug encodings.
     """
-    
+
     working_encodings = defaultdict(list)
     matching_encodings = []
-    
+
     decodings = encodings = set(aliases.values())
-    
+
     if encoding:
         encodings = (encoding,)
-        
+
     if decoding:
         decodings = (decoding,)
-    
+
     for encoding in encodings:
         for decoding in decodings:
             if encoding == decoding:
                 continue
             with suppress(UnicodeEncodeError, LookupError, UnicodeDecodeError):
                 values = values_to_test.encode(encoding).decode(decoding)
-                working = WorkingEncoding(encoding, decoding, values, bad_values)
+                working = WorkingEncoding(
+                    encoding, decoding, values, bad_values
+                )
                 working_encodings[values].append(working)
                 if values == bad_values:
                     matching_encodings.append(working)
-    
+
     return matching_encodings, working_encodings
 
-def parse_args() -> Namespace:
 
+def parse_args() -> Namespace:
     """
     This function parses command line arguments.
     """
-    
-    parser = ArgumentParser(description="This script helps you to debug encoding problems.")
+
+    parser = ArgumentParser(
+        description="This script helps you to debug encoding problems."
+    )
     encodings = parser.add_mutually_exclusive_group()
-    encodings.add_argument('--encoding', '-e', help='If you know what encoding this text is encoded with, specify it in this argument.')
-    encodings.add_argument('--decoding', '-d', help='If you know what encoding this text is decoded with, specify it in this argument.')
-    parser.add_argument('--bad-values', '--values', '-v', help='How tested values are printed when you have your encoding problems.')
-    parser.add_argument('--json', '-j', action="store_true", help='JSON output.')
-    parser.add_argument('value_to_test')
+    encodings.add_argument(
+        "--encoding",
+        "-e",
+        help="If you know what encoding this text is encoded with, specify it in this argument.",
+    )
+    encodings.add_argument(
+        "--decoding",
+        "-d",
+        help="If you know what encoding this text is decoded with, specify it in this argument.",
+    )
+    parser.add_argument(
+        "--bad-values",
+        "--values",
+        "-v",
+        help="How tested values are printed when you have your encoding problems.",
+    )
+    parser.add_argument(
+        "--json", "-j", action="store_true", help="JSON output."
+    )
+    parser.add_argument("value_to_test")
     return parser.parse_args()
-    
-def main() -> int:
 
+
+def main() -> int:
     """
     This function executes this script from the command line.
     """
-    
+
     arguments = parse_args()
-    matching_encodings, working_encodings = debug_encoding(arguments.value_to_test, arguments.bad_values, arguments.encoding, arguments.decoding)
+    matching_encodings, working_encodings = debug_encoding(
+        arguments.value_to_test,
+        arguments.bad_values,
+        arguments.encoding,
+        arguments.decoding,
+    )
 
     if matching_encodings:
         if arguments.json:
-            dump([{attr: getattr(encoding, attr) for attr in dir(encoding) if not attr.startswith("__") and not attr.endswith("__")} for encoding in matching_encodings ], stdout, indent=4)
+            dump(
+                [
+                    {
+                        attr: getattr(encoding, attr)
+                        for attr in dir(encoding)
+                        if not attr.startswith("__")
+                        and not attr.endswith("__")
+                    }
+                    for encoding in matching_encodings
+                ],
+                stdout,
+                indent=4,
+            )
             return 0
-        print("\n".join(
-            f'Encoding: {encoding.encoding!r}, '
-            f'Decoding: {encoding.decoding!r}, '
-            f'Output: {encoding.decoded_values!r}'
-            for encoding in matching_encodings
-        ))
+        print(
+            "\n".join(
+                f"Encoding: {encoding.encoding!r}, "
+                f"Decoding: {encoding.decoding!r}, "
+                f"Output: {encoding.decoded_values!r}"
+                for encoding in matching_encodings
+            )
+        )
         return 0
 
     if arguments.json:
-        dump({k: {attr: getattr(encoding, attr) for attr in dir(encoding) if not attr.startswith("__") and not attr.endswith("__")} for k, values in working_encodings.items() for encoding in values}, stdout, indent=4)
+        dump(
+            {
+                k: {
+                    attr: getattr(encoding, attr)
+                    for attr in dir(encoding)
+                    if not attr.startswith("__") and not attr.endswith("__")
+                }
+                for k, values in working_encodings.items()
+                for encoding in values
+            },
+            stdout,
+            indent=4,
+        )
         return 0
 
-    print("\n".join(
-        f'Output: {encoding.decoded_values!r}:\n\t'
-        f'Encoding: {encoding.encoding!r}, '
-        f'Decoding: {encoding.decoding!r}'
-        for encodings in working_encodings.values()
-        for encoding in encodings
-    ))
+    print(
+        "\n".join(
+            f"Output: {encoding.decoded_values!r}:\n\t"
+            f"Encoding: {encoding.encoding!r}, "
+            f"Decoding: {encoding.decoding!r}"
+            for encodings in working_encodings.values()
+            for encoding in encodings
+        )
+    )
     return 0
 
+
 if __name__ == "__main__":
     exit(main())
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Dict.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
 __all__ = ["cleandict", "copy_cleandict", "dict"]
 
 from collections.abc import Hashable, Iterator, Callable
 from typing import List, Dict, Any
 
 
 def cleandict(dict_: dict, keys: List[Hashable], invers: bool = False) -> dict:
-
     """
     This function clean a dictionary.
     """
 
     if invers:
         for key in keys:
             del dict_[key]
@@ -118,113 +117,100 @@
 
     for key in to_delete:
         del dict_[key]
     return dict_
 
 
 def copy_cleandict(dict_: dict, *args, **kwargs) -> dict:
-
     """
     This function copy and clean a dictionary.
 
     args and kwargs are passed to cleandict.
     """
 
     return cleandict(dict_.copy(), *args, **kwargs)
 
 
 class dict(dict):
     def __or__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> | <function>'.
         """
 
         return dict((k, other(k, v)) for k, v in self.items())
 
     def __ior__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> |= <function>'.
         """
 
         return dict((k, other(k, v)) for k, v in self.items())
 
     def __matmul__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> @ function'.
         """
 
         return dict((k, other(k)) for k in self.keys())
 
     def __imatmul__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> @= function'.
         """
 
         return dict((k, other(k)) for k in self.keys())
 
     def __invert__(self) -> Dict[Hashable, Any]:
-
         """
         This function implements '~<dict>'.
         """
 
         return dict((v, k) for k, v in self.items())
 
     def __inv__(self) -> Dict[Hashable, Any]:
-
         """
         This function implements '~<dict>'.
         """
 
         return dict((v, k) for k, v in self.items())
 
     def __rshift__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> >> function'.
         """
 
         return dict((k, other(v)) for k, v in self.items())
 
     def __irshift__(self, other: Callable) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> >> function'.
         """
 
         return dict((k, other(v)) for k, v in self.items())
 
     def __sub__(self, other: Iterator[Hashable]) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> - <Iterator>'
         """
 
         return dict((k, v) for k, v in self.items() if k not in other)
 
     def __isub__(self, other: Iterator[Hashable]) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> -= <Iterator>'
         """
 
         return dict((k, v) for k, v in self.items() if k not in other)
 
     def __add__(self, other: Iterator[Hashable]) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> + <Iterator>'
         """
 
         return dict((k, v) for k, v in self.items() if k in other)
 
     def __iadd__(self, other: Iterator[Hashable]) -> Dict[Hashable, Any]:
-
         """
         This function implements '<dict> += <Iterator>'
         """
 
         return dict((k, v) for k, v in self.items() if k in other)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/DictObject.py` & `PythonToolsKit-1.2.4/PythonToolsKit/DictObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
     """
     This class create object and sub-object from Json Structure.
     """
 
     def __init__(self, data: dict):
         if isinstance(data, dict):
-
             for key, value in data.items():
                 if isinstance(value, dict):
                     setattr(self, key.replace("-", "_"), DictObject(value))
                 else:
                     setattr(self, key.replace("-", "_"), value)
 
             dict_ = self._dict = self.__dict__
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Encodings.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Encodings.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 from locale import getpreferredencoding
 from contextlib import suppress
 from os import device_encoding
 from functools import partial
 
 
 def get_encodings():
-
     """
     This function returns the probable encodings.
 
     >>> [encoding for i, encoding in enumerate(get_encodings()) if i > 1]
     ['utf-8', 'cp1252', 'latin-1']
     >>>
     """
@@ -157,15 +156,14 @@
 
     yield "utf-8"  # Default for Linux
     yield "cp1252"  # Default for Windows
     yield "latin-1"  # Can read all files
 
 
 def decode_data(data: bytes) -> str:
-
     """
     This function decodes data (try some encodings).
 
     >>> len(decode_data(bytes(range(256))))
     256
     >>>
     """
@@ -193,28 +191,26 @@
 b64decode_file = decode
 
 b64encode_lines = encodebytes
 b64decode_lines = decodebytes
 
 
 def urlsafe_b64encode(data: bytes) -> bytes:
-
     """
     Same as base64.urlsafe_b64encode
 
     >>> urlsafe_b64encode(bytes(range(256)))
     b'AAECAwQFBgcICQoLDA0ODxAREhMUFRYXGBkaGxwdHh8gISIjJCUmJygpKissLS4vMDEyMzQ1Njc4OTo7PD0-P0BBQkNERUZHSElKS0xNTk9QUVJTVFVWV1hZWltcXV5fYGFiY2RlZmdoaWprbG1ub3BxcnN0dXZ3eHl6e3x9fn-AgYKDhIWGh4iJiouMjY6PkJGSk5SVlpeYmZqbnJ2en6ChoqOkpaanqKmqq6ytrq-wsbKztLW2t7i5uru8vb6_wMHCw8TFxsfIycrLzM3Oz9DR0tPU1dbX2Nna29zd3t_g4eLj5OXm5-jp6uvs7e7v8PHy8_T19vf4-fr7_P3-_w=='
     >>>
     """
 
     return b64encode(data).translate(_urlsafe_encode_translation)
 
 
 def urlsafe_b64decode(data: bytes) -> bytes:
-
     """
     Same as base64.urlsafe_b64decode
 
     >>> urlsafe_b64decode(b'AAECAwQFBgcICQoLDA0ODxAREhMUFRYXGBkaGxwdHh8gISIjJCUmJygpKissLS4vMDEyMzQ1Njc4OTo7PD0-P0BBQkNERUZHSElKS0xNTk9QUVJTVFVWV1hZWltcXV5fYGFiY2RlZmdoaWprbG1ub3BxcnN0dXZ3eHl6e3x9fn-AgYKDhIWGh4iJiouMjY6PkJGSk5SVlpeYmZqbnJ2en6ChoqOkpaanqKmqq6ytrq-wsbKztLW2t7i5uru8vb6_wMHCw8TFxsfIycrLzM3Oz9DR0tPU1dbX2Nna29zd3t_g4eLj5OXm5-jp6uvs7e7v8PHy8_T19vf4-fr7_P3-_w==')
     b'\\x00\\x01\\x02\\x03\\x04\\x05\\x06\\x07\\x08\\t\\n\\x0b\\x0c\\r\\x0e\\x0f\\x10\\x11\\x12\\x13\\x14\\x15\\x16\\x17\\x18\\x19\\x1a\\x1b\\x1c\\x1d\\x1e\\x1f !"#$%&\\'()*+,+./0123456789:;<=\\x0f\\xd0\\x10P\\x90\\xd1\\x11Q\\x91\\xd2\\x12R\\x92\\xd3\\x13S\\x93\\xd4\\x14T\\x94\\xd5\\x15U\\x95\\xd6\\x16V\\x96\\xd7\\x17W\\x97\\xd8\\x18X\\x98\\xd9\\x19Y\\x99\\xda\\x1aZ\\x9a\\xdb\\x1b[\\x9b\\xdc\\x1c\\\\\\x9c\\xdd\\x1d]\\x9d\\xde\\x1e^\\x9e\\xdf\\x1f/\\x9c\\x08\\x18(8HXhx\\x88\\x98\\xa8\\xb8\\xc8\\xd8\\xe8\\xf9\\t\\x19)9IYiy\\x89\\x99\\xa9\\xb9\\xc9\\xd9\\xe9\\xfa\\n\\x1a*:JZjz\\x8a\\x9a\\xaa\\xba\\xca\\xda\\xea\\xc2\\xc6\\xca\\xce\\xd2\\xd6\\xda\\xde\\xe2\\xe6\\xea\\xee\\xf2\\xf6\\xfa\\xc0\\xc1\\xc2\\xc3\\xc4\\xc5\\xc6\\xc7\\xc8\\xc9\\xca\\xcb\\xcc\\xcd\\xce\\xcf\\xd0\\xd1\\xd2\\xd3\\xd4\\xd5\\xd6\\xd7\\xd8\\xd9\\xda\\xdb\\xdc\\xdd\\xde\\xd88x\\xb8\\xf99y\\xb9\\x8e\\x9e\\xae\\xbe\\xce\\xde\\xee\\xff\\x0f\\x1f/\\x13\\xd7\\xdb\\xdf\\xe1\\xfa\\xfb?|'
     >>>
     """
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Function.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Function.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 __all__ = ["def_Function", "Function"]
 
 from collections.abc import Callable
 from typing import List, Any, Iterator
 
 
 def def_Function(function: Callable) -> Callable:
-
     """
     This decorator transform basic function in Function.
     """
 
     return Function(function)
 
 
@@ -86,14 +85,13 @@
     def __init__(self, function: Callable):
         self.function = function
 
     def __call__(self, *args, **kwargs) -> Any:
         return self.function(*args, **kwargs)
 
     def __lshift__(self, other: Iterator) -> List[Any]:
-
         """
         This function implements '<Function> << <Iterator>'.
         """
 
         function = self.function
         return [function(x) for x in other]
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/GetFile.py` & `PythonToolsKit-1.2.4/PythonToolsKit/GetFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 from platform import system
 import builtins
 
 system: str = system()
 
 
 def get_real_path(file_path: str, module_path: str = None) -> str:
-
     """
     This function researchs a file from current
     directory and lib directory.
     """
 
     if file_path is None:
         return file_path
@@ -101,14 +100,13 @@
     ):
         return module_file_path
 
     raise FileNotFoundError(f"No such file or directory: '{file_path}'")
 
 
 def open(file_path: str, *args, **kwargs) -> TextIOWrapper:
-
     """
     This function researchs a file from current
     directory and lib directory and open it.
     """
 
     return builtins.open(get_real_path(file_path), *args, **kwargs)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/GetPass.py` & `PythonToolsKit-1.2.4/PythonToolsKit/GetPass.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     from tty import setraw
 
     fileno = stdin.fileno
     read = stdin.buffer.read
     encoding = device_encoding(fileno())
 
     def getch() -> bytes:
-
         """
         This function gets input keyboard and return character.
         """
 
         fd = fileno()
         tty_attr = tcgetattr(fileno())
 
@@ -94,15 +93,14 @@
         finally:
             tcsetattr(fd, TCSADRAIN, tty_attr)
 
         return char
 
 
 def getpass(prompt: str = "Password: ", show: str = "*") -> str:
-
     """
     This function prompts for password and show "<show>".
     """
 
     password = []
     char = None
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/GetType.py` & `PythonToolsKit-1.2.4/PythonToolsKit/GetType.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
     value: str,
     raise_exception: bool = True,
     default: Any = None,
     case_sensitive: bool = False,
     true_values: Iterator[str] = ("yes", "on", "1", "true", "y"),
     false_values: Iterator[str] = ("no", "off", "0", "false", "n"),
 ) -> None:
-
     """
     This function returns a boolean from string value.
 
     >>> import GetType
     >>> GetType.get_boolean('true')
     True
     >>> GetType.get_boolean('yes')
@@ -214,15 +213,14 @@
             f"{value!r} is not in {list(false_values) + list(true_values)!r}"
         )
     else:
         return default
 
 
 def is_number(value: str, raise_exception: bool) -> bool:
-
     """
     This function checks value for valid number.
 
     >>> import GetType
     >>> GetType.is_number("1", True)
     True
     >>> GetType.is_number("1.1", True)
@@ -245,15 +243,14 @@
     else:
         return False
 
 
 def get_step(
     value: str, step_char: str, step_default: int, raise_exception: bool
 ) -> Tuple[float, str]:
-
     """
     This function returns the step value.
 
     >>> import GetType
     >>> GetType.get_step("0-5:1", ":", 1, True)
     (1.0, '0-5')
     >>> GetType.get_step("0-5?1.1", "?", 1, True)
@@ -277,15 +274,14 @@
         else:
             return step_default, values
     else:
         return step_default, value
 
 
 def drange(start: float, stop: float, step: float = 1) -> Iterator[float]:
-
     """
     This function implements range for Decimal value.
 
     >>> import GetType
     >>> for i in GetType.drange(0, 5, 2): i
     ...
     0.0
@@ -316,15 +312,14 @@
     default: Any = None,
     separator: str = ",",
     step_char: str = ":",
     step_default: int = 1,
     generator_char: str = "-",
     raise_exception: bool = True,
 ) -> Iterator[float]:
-
     """
     This function yields integers from string value.
 
     >>> import GetType
     >>> [i for i in GetType.get_numbers("4")]
     [4.0]
     >>> [i for i in GetType.get_numbers("4.1")]
@@ -396,15 +391,14 @@
             )
 
         elif default is not None:
             yield default
 
 
 def try_type(value: str) -> Any:
-
     """
     This function returns a typed value (be careful with this function,
     detection can be bad (example: if you want a string of number this
     function will return a float)).
 
     >>> import GetType
     >>> GetType.try_type("1")
@@ -451,15 +445,14 @@
     elif not value or value_ == "null" or value_ == "none":
         return None
     else:
         return value
 
 
 def is_ip(value: str, raise_exception: bool) -> bool:
-
     """
     This function valids IPv4 addresses.
 
     >>> import GetType
     >>> GetType.is_ip("0.0.0.0", True)
     True
     >>> GetType.is_ip("255.255.255.255", True)
@@ -513,15 +506,14 @@
             else:
                 return False
 
     return True
 
 
 def get_ips(ip1: ip_address, ip2: ip_address) -> Iterator[ip_address]:
-
     """
     This function yields IP addresses from first IP to second.
 
     >>> import GetType
     >>> [str(i) for i in GetType.get_ips(ip_address("10.10.10.0"), ip_address("10.10.10.10"))]
     ['10.10.10.0', '10.10.10.1', '10.10.10.2', '10.10.10.3', '10.10.10.4', '10.10.10.5', '10.10.10.6', '10.10.10.7', '10.10.10.8', '10.10.10.9']
     >>> [str(i) for i in GetType.get_ips(ip_address("10.10.10.10"), ip_address("10.10.10.0"))]
@@ -542,15 +534,14 @@
 def get_ipv4_addresses(
     value: str,
     default: Any = None,
     separator: str = ",",
     generator_char: str = "-",
     raise_exception: bool = True,
 ) -> Iterator[IPv4Address]:
-
     """
     This function yields ip addresses.
 
     >>> import GetType
     >>> [str(i) for i in GetType.get_ipv4_addresses("10.10.10.10-10.10.10.0")]
     ['10.10.10.0', '10.10.10.1', '10.10.10.2', '10.10.10.3', '10.10.10.4', '10.10.10.5', '10.10.10.6', '10.10.10.7', '10.10.10.8', '10.10.10.9']
     >>> [str(i) for i in GetType.get_ipv4_addresses("10.10.10.0/29")]
@@ -593,15 +584,14 @@
             "separator/generator_char should not be '/' (reserved by network)"
         )
 
     ips = value.split(separator)
 
     for ip in ips:
         if "/" in ip:
-
             ip_, network = ip.split("/", 1)
             if (
                 is_ip(ip_, raise_exception)
                 and network.isdigit()
                 and 0 <= int(network) <= 32
             ):
                 yield from IPv4Network(ip).hosts()
@@ -610,15 +600,14 @@
                     f"{ip!r} is not a valid network (example: 127.0.0.1/29)"
                     " [<valid ip>/<0-32>]."
                 )
             elif default is not None:
                 yield default
 
         elif generator_char in ip:
-
             value1, value2 = ip.split(generator_char, 1)
             if is_ip(value1, raise_exception) or is_ip(
                 value2, raise_exception
             ):
                 ip1 = IPv4Address(value1)
                 ip2 = IPv4Address(value2)
                 yield from get_ips(ip1, ip2)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Import.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Import.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,24 +51,22 @@
 from importlib.util import spec_from_file_location, module_from_spec
 from os.path import basename, splitext
 from importlib._bootstrap import _exec
 from types import ModuleType
 
 
 def reload(module: ModuleType) -> ModuleType:
-
     """
     This function reload a module.
     """
 
     return _exec(module.__spec__, module)
 
 
 def import_from_filename(filename: str) -> ModuleType:
-
     """
     This function returns a module from path/filename.
     """
 
     spec = spec_from_file_location(splitext(basename(filename))[0], filename)
     module = module_from_spec(spec)
     module.__spec__ = spec
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Json.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Json.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,14 @@
 	qwerty
 	\"\"\",
 	15,45: 15,45,
 }"""
 
 
 def get_valid_json(json: str) -> str:
-
     """
     This function returns a valid JSON from invalid JSON.
 
     >>> from Json import invalid_json_example1, invalid_json_example2
     >>> from Json import get_valid_json, load_invalid_json
     >>> from json import loads
     >>> loads(get_valid_json(invalid_json_example1))
@@ -136,15 +135,14 @@
     json = regex_simplequote1.sub(r'"\g<1>', json, count=0)
     json = regex_simplequote2.sub(r'\g<1>"', json, count=0)
 
     return json
 
 
 def load_invalid_json(json: str) -> Any:
-
     """
     This function load invalid JSON.
 
     >>> from Json import invalid_json_example1, invalid_json_example2
     >>> from Json import get_valid_json, load_invalid_json
     >>> from json import loads
     >>> load_invalid_json(invalid_json_example2)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/List.py` & `PythonToolsKit-1.2.4/PythonToolsKit/List.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,54 +78,48 @@
 
 from collections.abc import Callable, Iterator
 from typing import List, Any
 
 
 class list(list):
     def __or__(self, other: Callable) -> List[Any]:
-
         """
         This function implements '<list> | <function>'.
         """
 
         return [other(x) for x in self]
 
     def __ior__(self, other: Callable) -> List[Any]:
-
         """
         This function implements '<list> |= <function>'.
         """
 
         return [other(x) for x in self]
 
     def __invert__(self) -> List[Any]:
-
         """
         This function implements '~<list>'.
         """
 
         return self[::-1]
 
     def __inv__(self) -> List[Any]:
-
         """
         This function implements '~<list>'.
         """
 
         return self[::-1]
 
     def __sub__(self, other: Iterator[Any]) -> List[Any]:
-
         """
         This function implements '<list> - <Iterator>'
         """
 
         return [x for x in self if x not in other]
 
     def __isub__(self, other: Iterator[Any]) -> List[Any]:
-
         """
         This function implements '<list> -= <Iterator>'
         """
 
         [self.remove(x) for x in other]
         return self
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Logs.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Logs.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 from os.path import exists
 from gzip import compress
 from io import StringIO
 from os import remove
 
 
 def get_custom_logger(name: str = None) -> Logger:
-
     """
     This function create a custom logger.
     """
 
     logger = getLogger(name or _getframe().f_code.co_filename)
     logger.propagate = False
 
@@ -134,15 +133,14 @@
 addLevelName(5, "TRACE")
 
 logger.trace: Callable = lambda x: logger_log(5, x)
 logger_trace: Callable = logger.trace
 
 
 def log_trace(function: FunctionType) -> FunctionType:
-
     """
     This decorator trace functions (start and end).
     """
 
     @wraps(function)
     def wrapper(*args, **kwds):
         name = function.__name__
@@ -166,15 +164,14 @@
         self.getlog = output.getvalue
         self.trunc = output.truncate
         self.seek = output.seek
         writer_ = self.writer = writer(output, quoting=QUOTE_ALL)
         self.writerow = writer_.writerow
 
     def format(self, record):
-
         """
         This function formats record in CSV.
         """
 
         time_ = gmtime(record.created)
         date = asctime(time_)
         time_ = strftime("%Y-%m-%d %H:%M:%S", time_)
@@ -213,62 +210,56 @@
         self._debug = logger.debug
         self._info = logger.info
         self._warning = logger.warning
         self._error = logger.error
         self._critical = logger.critical
 
     def debug(self, log: str) -> None:
-
         """
         This function logs a colored debug message.
         """
 
         self._debug(f"\x1b[32m{log}\x1b[0m")
 
     def info(self, log: str) -> None:
-
         """
         This function logs a colored info message.
         """
 
         self._info(f"\x1b[34m{log}\x1b[0m")
 
     def warning(self, log: str) -> None:
-
         """
         This function logs a colored warning message.
         """
 
         self._warning(f"\x1b[33m{log}\x1b[0m")
 
     def error(self, log: str) -> None:
-
         """
         This function logs a colored error message.
         """
 
         self._error(f"\x1b[35m{log}\x1b[0m")
 
     def critical(self, log: str) -> None:
-
         """
         This function logs a colored critical message.
         """
 
         self._critical(f"\x1b[31m{log}\x1b[0m")
 
 
 class CompressLogHandler(RotatingFileHandler):
 
     """
     This class implements a handler to compress and rotate log files.
     """
 
     def doRollover(self):
-
         """
         Do a rollover, as described in __init__().
         """
 
         stream = self.stream
 
         if stream:
@@ -285,23 +276,21 @@
 
             self.rotate(base_filename, filename)
 
         if not self.delay:
             stream = self._open()
 
     def namer(self, name: str) -> str:
-
         """
         This function returns the new name of the old log files.
         """
 
         return f"{name}.gz"
 
     def rotator(self, source: str, destination: str) -> None:
-
         """
         This function compresses old log files.
         """
 
         with open(source, "rb") as source_file:
             compressed = compress(source_file, 9)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/OrdDict.py` & `PythonToolsKit-1.2.4/PythonToolsKit/OrdDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,33 +346,30 @@
 
         raise StopIteration
 
     def __iter__(self) -> Iterable[Tuple[Hashable, Any]]:
         yield from ((key, self.dict[key]) for key in self.list)
 
     def to_dict(self) -> Dict[Hashable, Any]:
-
         """
         This method returns a dict from OrdDict instance.
         """
 
         return {key: self.dict[key] for key in self.list}
 
     def add(self, item: Hashable, value: Any) -> None:
-
         """
         This method adds an item to OrdDict instance.
         """
 
         self[item] = value
 
     def insert(
         self, index: int, item: Hashable, value: Any, error: bool = True
     ) -> None:
-
         """
         This method inserts an item in 'index' position.
         """
 
         try:
             self.dict[item]
         except KeyError:
@@ -382,15 +379,14 @@
             if error:
                 raise ValueError(f"Can't insert {item!r}, item exists.")
             self.list.remove(item)
             self.list.insert(index, item)
             self.dict[item] = value
 
     def modify(self, item: Hashable, value: Any, error: bool = True) -> None:
-
         """
         This method updates value for an item.
         """
 
         try:
             self.dict[item]
         except KeyError:
@@ -399,202 +395,181 @@
                     f"Can't modify {item!r}, item doesn't exists."
                 )
             self.list.append(item)
 
         self.dict[item] = value
 
     def move(self, index: int, item: Hashable) -> None:
-
         """
         This method moves an item.
         """
 
         self.list.remove(item)
         self.list.insert(index, item)
 
     def delete(self, item: Hashable) -> None:
-
         """
         This method deletes an item.
         """
 
         del self.dict[item]
         self.list.remove(item)
 
     def values(self) -> Iterable[Any]:
-
         """
         This method yields values.
         """
 
         yield from (self.dict[key] for key in self.list)
 
     def keys(self) -> Iterable[Hashable]:
-
         """
         This method yields keys.
         """
 
         yield from (key for key in self.list)
 
     def items(self) -> Iterable[Tuple[Hashable, Any]]:
-
         """
         This method yields keys and values.
         """
 
         yield from ((key, self.dict[key]) for key in self.list)
 
     def get(self, item: Hashable) -> Any:
-
         """
         This method returns the value from item
         """
 
         return self.dict[item]
 
     def setdefault(self, item: Hashable, value: Any) -> Any:
-
         """
         This method sets the value and returns it or returns the value.
         """
 
         try:
             value = self.dict[item]
         except KeyError:
             self.dict[item] = value
             self.list.append(item)
 
         return value
 
     def index(self, item: Hashable) -> int:
-
         """
         This method returns the position's key.
         """
 
         return self.list.index(item)
 
     def index_value(self, index: int) -> Any:
-
         """
         This method returns the value's position.
         """
 
         return self.dict[self.list[index]]
 
     def index_key(self, index: int) -> Hashable:
-
         """
         This method returns the item's position.
         """
 
         return self.list[index]
 
     def get_key_value(self, index: int) -> Tuple[Hashable, Any]:
-
         """
         This method returns item and value from index.
         """
 
         key = self.list[index]
         return key, self.dict[key]
 
     def remove(self, index: int) -> None:
-
         """
         This method deletes items from index.
         """
 
         key = self.list.pop(index)
         del self.dict[key]
 
     def reverse(self) -> None:
-
         """
         This method deletes items from index.
         """
 
         self.list.reverse()
 
     def copy(self) -> OrdDict:
-
         """
         This method returns an OrdDict with
         same postions, keys and values.
         """
 
         return OrdDict(self.to_dict())
 
     def update(self, dict_: Dict[Hashable, Any]) -> Any:
-
         """
         This method changes values or adds items
         from a dict.
         """
 
         for key, value in dict_.items():
             try:
                 self.dict[key]
             except KeyError:
                 self.list.append(key)
 
             self.dict[key] = value
 
     def clear(self) -> None:
-
         """
         This method clears OrdDict.
         """
 
         self.list.clear()
         self.dict.clear()
 
     def extend(self, dict_: Dict[Hashable, Any]) -> None:
-
         """
         This method setdefaults all keys and values from dict.
         """
 
         for key, value in dict_.items():
             try:
                 self.dict[key]
             except KeyError:
                 self.dict[key] = value
                 self.list.append(key)
 
     def pop(self, item: Hashable) -> Any:
-
         """
         This method deletes and returns a value from item.
         """
 
         self.list.remove(item)
         return self.dict.pop(item)
 
     def popitem(self) -> Tuple[Hashable, Any]:
-
         """
         This method deletes and returns the last key and value.
         """
 
         key = self.list.pop()
         return key, self.dict.pop(key)
 
     def pop_index(self, index: int = -1) -> Tuple[Hashable, Any]:
-
         """
         This method deletes and returns key and value from index.
         """
 
         key = self.list.pop(index)
         return key, self.dict.pop(key)
 
     def sort(self) -> None:
-
         """
         This method sorts OrdDict by keys.
         """
 
         self.list.sort()
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/PrintF.py` & `PythonToolsKit-1.2.4/PythonToolsKit/PrintF.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
     start: str = "",
     end: str = "\n",
     progressbar: ProgressBar = ProgressBar,
     add_progressbar: bool = True,
     oneline_progress: bool = False,
     **kwargs,
 ) -> None:
-
     """
     This function prints formatted and colored information and progression.
     """
 
     show, color = states_get(state) or ("[ ]", "\x1b[39m")
 
     progress_bar = ""
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Process.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Process.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 from threading import Timer
 from typing import Tuple
 
 
 def real_time_process_output(
     *args, input: bytes = b"", timeout: int = 0, **kwargs
 ) -> Iterator[Tuple[bytes, bytes, int]]:
-
     """
     This function returns lines of process in real time.
 
     args and kwargs are sent to subprocess.Popen.
     """
 
     process = Popen(*args, stdin=PIPE, stdout=PIPE, stderr=PIPE, **kwargs)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Random.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Random.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 from collections.abc import Callable
 from random import randint, choices
 
 
 def get_number_function(
     numbers: Union[int, Tuple[int, int]], secure: bool = False
 ) -> Callable:
-
     """
     This function returns a function to get (random) number.
     """
 
     if isinstance(numbers, int):
         return lambda: numbers
     elif secure:
@@ -120,15 +119,14 @@
     characters: str = printable[:-5],
     letters: bool = False,
     alphanumeric: bool = False,
     ascii: bool = False,
     latin1: bool = False,
     check_strong: bool = False,
 ) -> Union[str, List[str]]:
-
     """
     This function generates random strings.
     """
 
     if letters:
         chars = ascii_letters
     elif alphanumeric:
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/RecursionDebug.py` & `PythonToolsKit-1.2.4/PythonToolsKit/RecursionDebug.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 from warnings import warn
 import sys
 
 
 def recurse_excepthook(
     exception_type: type, message: str, traceback: TracebackType
 ):
-
     """
     This function helps you to debug RecursionError.
     """
 
     if exception_type is RecursionError:
         counter = 0
         while traceback := getattr(traceback, "tb_next", None):
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Report.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Report.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,26 +159,24 @@
 if __package__:
     from .StringF import strings_tableformat
 else:
     from StringF import strings_tableformat
 
 
 def default_key_function(dict_: dict, attribute: str = None) -> Any:
-
     """
     This is a key function for sorted or filter function.
     """
 
     return dict_[attribute]
 
 
 def customfilter(
     function: Callable, objects: Sequence[dict]
 ) -> Tuple[List[dict], List[dict]]:
-
     """
     This function applies a filter on the data.
     """
 
     new_data = []
     filtered = []
     for object_ in objects:
@@ -201,15 +199,14 @@
         data: Union[dict, object],
         columns: Tuple[str] = ("keys", "values"),
     ):
         self.data = next(Report.get_dicts((data,)))
         self.columns = columns
 
     def report_text(self) -> str:
-
         """
         This function reports dict as text (Makdown).
         """
 
         data = self.data
         key, value = columns = self.columns
         keys = list(data.keys())
@@ -230,29 +227,27 @@
         return strings_tableformat(
             zip(keys, values),
             columns=self.columns,
             length=(max_keys, max_values),
         )
 
     def report_CSV(self, *args, **kwargs) -> str:
-
         """
         This function reports dict as CSV.
 
         *args and **kwargs are optional arguments for csv.writer
         """
 
         report = StringIO()
         csv_report = writer(report, *args, **kwargs)
         csv_report.writerow(self.columns)
         csv_report.writerows(self.data.items())
         return report.getvalue()
 
     def report_HTML(self) -> str:
-
         """
         This function reports dict as HTML.
         """
 
         html = (
             "<table><thead><tr><th>"
             + "</th><th>".join(self.columns)
@@ -264,15 +259,14 @@
             html += (
                 "<tr><td>" + str(key) + "</td><td>" + str(value) + "</td></tr>"
             )
 
         return html + "</tbody><tfoot></tfoot></table>"
 
     def report_JSON(self, *args, indent=4, **kwargs) -> str:
-
         """
         This function reports dict as JSON.
         """
 
         return dumps(self.data, *args, indent=indent, **kwargs)
 
 
@@ -316,15 +310,14 @@
 
         self.report_markdown = partial(self.report_text, delimiter="|")
 
     @staticmethod
     def get_dicts(
         objects: Union[Sequence[dict], Sequence[object]]
     ) -> Iterator[dict]:
-
         """
         This function returns dict from dict or object.
         """
 
         for object_ in objects:
             if isinstance(object_, dict):
                 yield object_
@@ -334,15 +327,14 @@
                     for k, v in object_.__dict__.items()
                     if not isinstance(v, Callable)
                 }
 
     def frequence(
         self, filtered: bool = False, pourcent: bool = True
     ) -> float:
-
         """
         This function returns the frequence of used/filtered objects
         for report.
         """
 
         objects, other = (
             (self.filtered, self.objects)
@@ -355,15 +347,14 @@
 
         number = len(objects)
         total = number + len(other)
 
         return (number / total * 100) if pourcent else (number / total)
 
     def report_text(self, *args, filtered: bool = False, **kwargs) -> str:
-
         """
         This function returns a text table to report
         objects.
 
         *args and **kwargs are sent to StringF.strings_tableformat
         """
 
@@ -375,15 +366,14 @@
         columns = objects[0].keys()
 
         return strings_tableformat(
             [o.values() for o in objects], columns=columns, *args, **kwargs
         )
 
     def report_HTML(self, filtered: bool = False):
-
         """
         This function returns a text table to report
         objects.
         """
 
         objects = self.filtered if filtered else self.objects
 
@@ -406,15 +396,14 @@
         body += "</tbody><tfoot></tfoot>"
 
         return f"<table>{columns}{body}</table>"
 
     def report_JSON(
         self, *args, filtered: bool = False, indent: int = 4, **kwargs
     ) -> str:
-
         """
         This function returns a JSON array of dict to report
         objects.
 
         *args and **kwargs are sent to json.dumps
         """
 
@@ -422,15 +411,14 @@
 
         if not objects:
             return None
 
         return dumps(objects, *args, indent=indent, **kwargs)
 
     def report_CSV(self, *args, filtered: bool = False, **kwargs):
-
         """
         This function returns a CSV content to report
         objects.
 
         *args and **kwargs are sent to DictWriter.writerows
         """
 
@@ -446,15 +434,14 @@
         csv_report.writeheader()
         csv_report.writerows(objects)
         return report.getvalue()
 
     def statistic(
         self, attributes: Sequence[str] = None, filtered: bool = False
     ) -> List[Dict[str, Union[str, int]]]:
-
         """
         This function returns statistics to report
         objects statistics.
         """
 
         objects = self.filtered if filtered else self.objects
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/StringF.py` & `PythonToolsKit-1.2.4/PythonToolsKit/StringF.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 from collections.abc import Iterator, Sequence
 from typing import Union
 
 
 def string_lengthformat(
     string: str, length: int = 13, end: str = "...", separator: str = ","
 ) -> str:
-
     """
     This function formats string length.
 
     >>> string_lengthformat("azerty")
     'azerty       ,'
     >>> string_lengthformat("azertyazertyazerty")
     'azertyazer...,'
@@ -133,15 +132,14 @@
 def strings_tableformat(
     strings: Iterator[Iterator[str]],
     length: Union[Sequence[int], int] = 13,
     end: str = "...",
     separator: str = "|",
     columns: Iterator[str] = None,
 ) -> str:
-
     """
     This function returns a formatted table of strings.
 
     >>> print(strings_tableformat([(0, 1), ("a" * 50, "b" * 50)]))
     |0            |1            |
     |aaaaaaaaaa...|bbbbbbbbbb...|
     >>> print(strings_tableformat([(0, 1), ("a" * 50, "b" * 50)], length=[13, 26]))
@@ -187,15 +185,14 @@
                 string_lengthformat("-" * size, size, end, separator)
             )
 
         table.append(first_line)
         table.append(second_line)
 
     for string_iter in strings:
-
         line = [separator]
         for string in string_iter:
             line.append(
                 string_lengthformat(string, get_length(), end, separator)
             )
 
         table.append(line)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Terminal.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ###################
 #    This package implements tools to build python package and tools.
-#    Copyright (C) 2022  Maurice Lambert
+#    Copyright (C) 2022, 2023  Maurice Lambert
 
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
 #    This program is distributed in the hope that it will be useful,
@@ -19,27 +19,27 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This package implements tools to build python package and tools.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/PythonToolsKit"
 
 copyright = """
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
+PythonToolsKit  Copyright (C) 2022, 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
 """
 __license__ = license
 __copyright__ = copyright
 
@@ -88,171 +88,154 @@
     """
 
     #############
     #  \x0X
     #############
 
     def bell() -> None:
-
         """
         This function play system sound.
         """
 
         stdout_write("\x07")
         stdout_flush()
 
     def backspace() -> None:
-
         """
         This function places the cursor on the precedent character.
         """
 
         stdout_write("\x08")
         stdout_flush()
 
     def tab() -> None:
-
         """
         This function places the cursor on the next multiple of 8.
         """
 
         stdout_write("\x09")
         stdout_flush()
 
     def line_feed() -> None:
-
         """
         This function places the cursor on the next line.
         """
 
         stdout_write("\x0A")
         stdout_flush()
 
     def carriage_return() -> None:
-
         """
         This function places the cursor on the first column.
         """
 
         stdout_write("\x0D")
         stdout_flush()
 
     #############
     #  \x1bX
     #############
 
     def save_position() -> None:
-
         """
         This function saves the cursor position.
         """
 
         stdout_write(f"{char_special_ANSI}7")
         stdout_flush()
 
     def restore_position() -> None:
-
         """
         This function restore the saved position.
         """
 
         stdout_write(f"{char_special_ANSI}8")
         stdout_flush()
 
     def clean() -> None:
-
         """
         This function cleans the console.
         """
 
         stdout_write(f"{char_special_ANSI}c")
         stdout_flush()
 
     #############
     #  \x1b[X
     #############
 
     def cursor_up(n: int = 0) -> None:
-
         """
         This function go to the precedent line
         (keep the same position on the precedent line).
         """
 
         stdout_write(f"{char_ANSI}{n}A")
         stdout_flush()
 
     def cursor_down(n: int = 0) -> None:
-
         """
         This function got to the next line
         (keep the same position on the next line).
         """
 
         stdout_write(f"{char_ANSI}{n}B")
         stdout_flush()
 
     def cursor_forward(n: int = 0) -> None:
-
         """
         This function go to the next character.
         """
 
         stdout_write(f"{char_ANSI}{n}C")
         stdout_flush()
 
     def cursor_back(n: int = 0) -> None:
-
         """
         This function go to the precedent character.
         """
 
         stdout_write(f"{char_ANSI}{n}D")
         stdout_flush()
 
     def cursor_next_line(n: int = 0) -> None:
-
         """
         This function go to the next line
         (on the first character of the next line).
         """
 
         stdout_write(f"{char_ANSI}{n}E")
         stdout_flush()
 
     def cursor_previous_line(n: int = 0) -> None:
-
         """
         This function go to the precedent line
         (on the first character of the precedent line).
         """
 
         stdout_write(f"{char_ANSI}{n}F")
         stdout_flush()
 
     def cursor_horizontal_absolute(n: int = 0) -> None:
-
         """
         This function go to the start of the line.
         """
 
         stdout_write(f"{char_ANSI}{n}G")
         stdout_flush()
 
     def cursor_position(line: int, position: int) -> None:
-
         """
         This function go to line:position.
         """
 
         stdout_write(f"{char_ANSI}{line};{position}H")
         stdout_flush()
 
     def erase_in_display(mode: int = 0) -> None:
-
         """
         This function clears a part of the screen.
 
         mode == 0 -> clear screen between cursor and end.
         mode == 1 -> clear screen between cursor and start.
         mode == 2 -> clear screen.
         mode == 3 -> clear screen and saved buffer.
@@ -263,53 +246,48 @@
                 "Mode should be an integer between 0 and 3 (include)."
             )
 
         stdout_write(f"{char_ANSI}{mode}J")
         stdout_flush()
 
     def erase_in_line(n: int = 0) -> None:
-
         """
         This function clears a part of the line.
         """
 
         stdout_write(f"{char_ANSI}{n}K")
         stdout_flush()
 
     def scroll_up(n: int = 0) -> None:
-
         """
         This function scroll whole page up.
         """
 
         stdout_write(f"{char_ANSI}{n}S")
         stdout_flush()
 
     def scroll_down(n: int = 0) -> None:
-
         """
         This function scroll whole page down.
         """
 
         stdout_write(f"{char_ANSI}{n}T")
         stdout_flush()
 
     def cursor_horizontale_verticale_position(
         line: int, position: int
     ) -> None:
-
         """
         This function go to line:position.
         """
 
         stdout_write(f"{char_ANSI}{line};{position}f")
         stdout_flush()
 
     def device_status_report() -> Tuple[bytes, bytes]:
-
         """
         This function reports the cursor position.
         """
 
         stdout_write(f"{char_ANSI}6n")
         stdout_flush()
 
@@ -329,238 +307,214 @@
             data = reader(1)
 
         position += data
 
         return precedent, position
 
     def save_current_cursor_position() -> None:
-
         """
         This function save the cursor position.
         """
 
         stdout_write(f"{char_ANSI}s")
         stdout_flush()
 
     def restore_saved_cursor_position() -> None:
-
         """
         This function save the cursor position.
         """
 
         stdout_write(f"{char_ANSI}u")
         stdout_flush()
 
     #############
     #  \x1b[Xm  (GRAPHIC)
     #############
 
     def reset() -> None:
-
         """
         This function resets colors (background and foreground).
         """
 
         stdout_write(f"{char_ANSI}0m")
         stdout_flush()
 
     def bold() -> None:
-
         """
         This function adds bold.
         """
 
         stdout_write(f"{char_ANSI}1m")
         stdout_flush()
 
     def faint() -> None:
-
         """
         This function adds intensity.
         """
 
         stdout_write(f"{char_ANSI}2m")
         stdout_flush()
 
     def italic() -> None:
-
         """
         This function adds italic.
         """
 
         stdout_write(f"{char_ANSI}3m")
         stdout_flush()
 
     def underline() -> None:
-
         """
         This function adds underline.
         """
 
         stdout_write(f"{char_ANSI}4m")
         stdout_flush()
 
     def slow_blink() -> None:
-
         """
         Sets blinking to less than 150 times per minute.
         """
 
         stdout_write(f"{char_ANSI}5m")
         stdout_flush()
 
     def rapid_blink() -> None:
-
         """
         Sets blinking to greter than 150 times per minute.
         """
 
         stdout_write(f"{char_ANSI}6m")
         stdout_flush()
 
     def reverse() -> None:
-
         """
         This function reverses colors (background/foreground).
         """
 
         stdout_write(f"{char_ANSI}7m")
         stdout_flush()
 
     def hide() -> None:
-
         """
         This function adds hide.
         """
 
         stdout_write(f"{char_ANSI}8m")
         stdout_flush()
 
     def strike() -> None:
-
         """
         Characters legible but marked as if for deletion.
         """
 
         stdout_write(f"{char_ANSI}9m")
         stdout_flush()
 
     def font(font: int) -> None:
-
         """
         This function changes font.
         """
 
         if font > 9:
             raise ValueError(f"font ({font}) should be smaller than 10")
 
         font += 10
         stdout_write(f"{char_ANSI}{font}m")
         stdout_flush()
 
     def gothic() -> None:
-
         """
         Characters legible but marked as if for deletion.
         """
 
         stdout_write(f"{char_ANSI}20m")
         stdout_flush()
 
     def no_bold() -> None:
-
         """
         This function removes bold.
         """
 
         stdout_write(f"{char_ANSI}21m")
         stdout_flush()
 
     def no_intensity() -> None:
-
         """
         This function removes intensity.
         """
 
         stdout_write(f"{char_ANSI}22m")
         stdout_flush()
 
     def no_italic() -> None:
-
         """
         This function removes italic.
         """
 
         stdout_write(f"{char_ANSI}23m")
         stdout_flush()
 
     def no_underline() -> None:
-
         """
         This function removes underline.
         """
 
         stdout_write(f"{char_ANSI}24m")
         stdout_flush()
 
     def no_blink() -> None:
-
         """
         This function removes underline.
         """
 
         stdout_write(f"{char_ANSI}25m")
         stdout_flush()
 
     def no_reverse() -> None:
-
         """
         This function replace colors (background/foreground).
         """
 
         stdout_write(f"{char_ANSI}27m")
         stdout_flush()
 
     def no_hide() -> None:
-
         """
         This function removes hide.
         """
 
         stdout_write(f"{char_ANSI}28m")
         stdout_flush()
 
     def not_crossed_out() -> None:
-
         """
         This function removes hide.
         """
 
         stdout_write(f"{char_ANSI}29m")
         stdout_flush()
 
     def change_foreground_color_3bytes(
         red: int, green: int, blue: int
     ) -> None:
-
         """
         This function changes foreground color
         using the 3 bytes mode.
         """
 
         if red > 255 or green > 255 or blue > 255:
             raise ValueError(
                 f"colors ({red};{green};{blue}) should be in range of 0 to 255"
             )
 
         stdout_write(f"{char_ANSI}38;2;{red};{green};{blue}m")
         stdout_flush()
 
     def change_foreground_color_8bits(color: int) -> None:
-
         """
         This function changes foreground color
         using the 8 bits mode.
 
         2**3 == 8 -> RED
         2**3 == 8 -> GREEN
         2**2 == 4 -> BLUE
@@ -577,15 +531,14 @@
 
         stdout_write(f"{char_ANSI}38;5;{color}")
         stdout_flush()
 
     def change_background_color_3bytes(
         red: int, green: int, blue: int
     ) -> None:
-
         """
         This function changes background color
         using the 3 bytes mode.
         """
 
         if (
             red > 255
@@ -599,28 +552,26 @@
                 f"colors ({red};{green};{blue}) should be in range of 0 to 255"
             )
 
         stdout_write(f"{char_ANSI}48;2;{red};{green};{blue}m")
         stdout_flush()
 
     def change_background_color_8bits(color: int) -> None:
-
         """
         This function changes background color
         using the 8 bits mode.
         """
 
         if color > 255 or color < 0:
             raise ValueError(f"color ({color}) should be in range of 0 to 255")
 
         stdout_write(f"{char_ANSI}48;5;{color}")
         stdout_flush()
 
     def change_foreground_color(color: str, mode: int = 1) -> None:
-
         """
         This function changes foreground color.
         """
 
         color = color.upper()
 
         if mode == 1:
@@ -635,15 +586,14 @@
 
         color = colors_map[color].value
 
         stdout_write(f"{char_ANSI}{mode}{color}")
         stdout_flush()
 
     def change_background_color(color: str, mode: int = 1) -> None:
-
         """
         This function changes background color.
         """
 
         color = color.upper()
 
         if mode == 1:
@@ -658,30 +608,27 @@
 
         color = colors_map[color].value
 
         stdout_write(f"{char_ANSI}{mode}{color}")
         stdout_flush()
 
     def reset_background() -> None:
-
         """
         This function resets the background color.
         """
 
-        stdout_write(f"{char_ANSI}39m")
+        stdout_write(f"{char_ANSI}49m")
         stdout_flush()
 
     def reset_foreground() -> None:
-
         """
         This function resets the foreground color.
         """
 
-        stdout_write(f"{char_ANSI}49m")
+        stdout_write(f"{char_ANSI}39m")
         stdout_flush()
 
 
 if platform == "win32":
 
     class Terminal(Terminal):
-
         __doc__ = Terminal.__doc__
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/TestArguments.py` & `PythonToolsKit-1.2.4/PythonToolsKit/TestArguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/TestTimeout.py` & `PythonToolsKit-1.2.4/PythonToolsKit/TestTimeout.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
 if __name__ == "__main__":
     freeze_support()
     main2()
 
 
 class Test2:
-
     test_ = True
 
     def __init__(self):
         self.test = True
 
     @process_timeout(3)
     def test3(self, arg1, arg2, kwarg1=None, kwarg2=None):
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Thread.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,30 +76,27 @@
 
     def __init__(self, function: Callable, *args, **kwargs):
         Thread.__init__(self, target=function, args=args, kwargs=kwargs)
         self.start()
 
 
 def threadify(function: Callable) -> Callable:
-
     """
     This decorator implements a simple way to
     call a function in a new thread.
     """
 
     @wraps(function)
     def wrapper(*args, **kwargs) -> SimpleThread:
-
         return SimpleThread(function, *args, **kwargs)
 
     return wrapper
 
 
 def join_all():
-
     """
     This function get all threads and join it.
 
     The current thread and the main thread are exclude.
     """
 
     thread_current = current_thread()
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Timeout.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Timeout.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,29 +143,27 @@
 
 freeze_support()
 current_pid: str = str(getpid())
 pid: str = environ.setdefault("PID", current_pid)
 
 
 def thread_quit_timeout(function_name: str) -> None:
-
     """
     This function raise a TimeoutError in the current
     thread and a KeyboardInterrupt in the main thread.
     """
 
     try:
         raise TimeoutError(f'TimeoutError in "{function_name}"')
     except TimeoutError:
         stderr.write(format_exc())
         interrupt_main()
 
 
 def thread_timeout(seconds: int) -> Callable:
-
     """
     This decorator implements a function timeout.
     """
 
     def decorator(function: Callable) -> Callable:
         @wraps(function)
         def wrapper(*args, **kwargs) -> Any:
@@ -203,15 +201,14 @@
         self.method = method
         self.queue = queue
         self.args = args
         self.kwargs = kwargs
 
 
 def _process_timeout(process_obj: _ProcessObject) -> None:
-
     """
     This function puts state and output or error in Queue.
     """
 
     put = process_obj.queue.put
 
     try:
@@ -219,22 +216,20 @@
             (True, process_obj.method(*process_obj.args, **process_obj.kwargs))
         )
     except Exception as error:
         put((False, error))
 
 
 def process_timeout(seconds: int) -> Callable:
-
     """
     This decorator implements a function timeout.
     """
 
     def decorator(function: Callable) -> Callable:
         def wrapper(*args, **kwargs) -> Any:
-
             if type(function) == classmethod:
                 args = args[1:]
                 real_function = function.__func__
             else:
                 real_function = function
 
             name = real_function.__qualname__ or real_function.__name__
@@ -282,23 +277,21 @@
     return decorator
 
 
 if is_linux:
     __all__.append("signal_timeout")
 
     def signal_quit_timeout(signum, frame) -> None:
-
         """
         This function raise a TimeoutError.
         """
 
         raise TimeoutError()
 
     def signal_timeout(seconds: int) -> Callable:
-
         """
         This decorator implements a function timeout.
         """
 
         def decorator(function: Callable) -> Callable:
             @wraps(function)
             def wrapper(*args, **kwargs) -> Callable:
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/Tuple.py` & `PythonToolsKit-1.2.4/PythonToolsKit/Tuple.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,53 +79,47 @@
 
 from collections.abc import Callable, Iterator
 from typing import Tuple, Any
 
 
 class tuple(tuple):
     def __or__(self, other: Callable) -> Tuple[Any]:
-
         """
         This function implements '<tuple> | <function>'.
         """
 
         return tuple(other(x) for x in self)
 
     def __ior__(self, other: Callable) -> Tuple[Any]:
-
         """
         This function implements '<tuple> |= <function>'.
         """
 
         return tuple(other(x) for x in self)
 
     def __invert__(self) -> Tuple[Any]:
-
         """
         This function implements '~<tuple>'.
         """
 
         return self[::-1]
 
     def __inv__(self) -> Tuple[Any]:
-
         """
         This function implements '~<tuple>'.
         """
 
         return self[::-1]
 
     def __sub__(self, other: Iterator[Any]) -> Tuple[Any]:
-
         """
         This function implements '<tuple> - <Iterator>'
         """
 
         return tuple(x for x in self if x not in other)
 
     def __isub__(self, other: Iterator[Any]) -> Tuple[Any]:
-
         """
         This function implements '<tuple> -= <Iterator>'
         """
 
         return tuple(x for x in self if x not in other)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/WindowsTerminal.py` & `PythonToolsKit-1.2.4/PythonToolsKit/WindowsTerminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 delete_persistent_terminal_transparency = (
     persistent_terminal_transparency
 ) = (
     persistent_virtual_terminal
 ) = delete_persistent_virtual_terminal = lambda: None
 
 if name == "nt":
-
     from winreg import (
         CreateKey,
         OpenKey,
         SetValueEx,
         CloseKey,
         HKEY_CURRENT_USER,
         KEY_WRITE,
@@ -135,15 +134,14 @@
     STDOUT: int = GetStdHandle(-11)
     STDERR: int = GetStdHandle(-12)
 
     LWA_ALPHA: DWORD = DWORD(0x00000002)
     LWA_COLORKEY: DWORD = DWORD(0x00000001)
 
     def desactive_virtual_terminal() -> bool:
-
         """
         This function desactive terminal colors on Windows.
 
         >>> print("\\x1b[32mabc\\x1b[0m")
         ←[32mabc←[0m
         >>> active_virtual_terminal()
         True
@@ -169,15 +167,14 @@
         # if not SetConsoleMode(STDIN, default_in_mode):
         #    return False
 
         is_active = False
         return True
 
     def active_virtual_terminal() -> bool:
-
         """
         This function active terminal colors on Windows.
 
         return True on success and False on fail.
 
         doc: https://docs.microsoft.com/fr-fr/windows/console/console-virtual-terminal-sequences#code-try-1
 
@@ -218,15 +215,14 @@
         # if not SetConsoleMode(STDIN, new_in_mode):
         #    return False
 
         is_active = True
         return True
 
     def persistent_virtual_terminal() -> None:
-
         """
         This function adds a virtual terminal persistent
         configuration using the registry.
 
         >>> persistent_virtual_terminal()
         >>>
         """
@@ -234,15 +230,14 @@
         path = "Console"
         CreateKey(HKEY_CURRENT_USER, path)
         key = OpenKey(HKEY_CURRENT_USER, path, 0, KEY_WRITE)
         SetValueEx(key, "VirtualTerminalLevel", 0, REG_DWORD, 1)
         CloseKey(key)
 
     def delete_persistent_virtual_terminal() -> None:
-
         """
         This function deletes the virtual terminal persistent
         configuration using the registry.
 
         >>> delete_persistent_virtual_terminal()
         >>>
         """
@@ -250,15 +245,14 @@
         path = "Console"
         CreateKey(HKEY_CURRENT_USER, path)
         key = OpenKey(HKEY_CURRENT_USER, path, 0, KEY_WRITE)
         DeleteValue(key, "VirtualTerminalLevel")
         CloseKey(key)
 
     def persistent_terminal_transparency(level: int) -> None:
-
         """
         This function adds a terminal transparency persistent
         configuration using the registry.
 
         'level' argument should be an integer between 77-255
         (77 (0x4D) is the most transparent level and 255
         (0xFF) is the most opaque level)
@@ -270,15 +264,14 @@
         path = "Console"
         CreateKey(HKEY_CURRENT_USER, path)
         key = OpenKey(HKEY_CURRENT_USER, path, 0, KEY_WRITE)
         SetValueEx(key, "WindowAlpha", 0, REG_DWORD, 1)
         CloseKey(key)
 
     def delete_persistent_terminal_transparency() -> None:
-
         """
         This function deletes the terminal transparency
         persistent configuration using the registry.
 
         >>> delete_persistent_terminal_transparency()
         >>>
         """
@@ -286,15 +279,14 @@
         path = "Console"
         CreateKey(HKEY_CURRENT_USER, path)
         key = OpenKey(HKEY_CURRENT_USER, path, 0, KEY_WRITE)
         DeleteValue(key, "WindowAlpha")
         CloseKey(key)
 
     def set_terminal_transparency(level: int) -> bool:
-
         """
         This function sets the terminal transparency on Windows.
 
         'level' argument should be an integer between 0-255
         (0 is the most transparent level and
         255 is the most opaque level)
 
@@ -313,15 +305,14 @@
             active_windows, 0, BYTE(level), LWA_ALPHA
         ):
             return True
 
         return False
 
     def set_color_transparency(color: int) -> bool:
-
         """
         This function sets the transparent color of the window.
 
         'level' argument should be an integer between 0-4294967295
         (0 (0x00000000) is black, 16777215 (0x00FFFFFF) is white,
         255 (0x000000FF) is blue, 65280 (0x0000FF00) is green and
         16711680 (0x00FF0000) is red)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/__init__.py` & `PythonToolsKit-1.2.4/PythonToolsKit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This package implements tools to build python package and tools.
 """
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit/urlopen.py` & `PythonToolsKit-1.2.4/PythonToolsKit/urlopen.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,45 +97,41 @@
     307: HTTPRedirectHandler().http_error_302,
     401: HTTPBasicAuthHandler().http_error_401,
     407: ProxyBasicAuthHandler().http_error_407,
 }
 
 
 def httpcode(*args: Sequence[int]) -> Callable:
-
     """
     This decorator change action on HTTP error
     code.
     """
 
     def decorator(function: Callable) -> Callable:
-
         for code in args:
             FUNCTIONS_CODES[code] = function
 
         return function
 
     return decorator
 
 
 class OpenerDirector(_OpenerDirector):
     def open(self, *args, context: SSLContext = None, **kwargs) -> Any:
-
         """
         This function implements the default URL opener.
         """
 
         if context is not None:
             self.handlers[-1]._context = context
 
         return super(OpenerDirector, self).open(*args, **kwargs)
 
 
 def build_opener(functions: Dict[int, Callable] = None) -> OpenerDirector:
-
     """
     This function creates an opener object
     using default handlers.
     """
 
     opener = OpenerDirector()
     add_handler = opener.add_handler
@@ -163,35 +159,32 @@
     auth_header = "Authorization"
 
     def __init__(self, functions: Dict[int, Callable] = None):
         functions = self.functions = functions or FUNCTIONS_CODES.copy()
         self.functions_get = functions.get
 
     def httpcode(self, *args: Sequence[int]) -> Callable:
-
         """
         This decorator change action on HTTP error
         code.
         """
 
         def decorator(function: Callable) -> Callable:
-
             for code in args:
                 FUNCTIONS_CODES[code] = function
 
             return function
 
         return decorator
 
     def http_response(
         self,
         request: Request,
         response: HTTPResponse,
     ) -> None:
-
         code: int = response.code
         message: str = response.msg
         headers: HTTPMessage = response.info()
         function = self.functions_get(code)
 
         instance = getattr(function, "__self__", None)
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit.egg-info/PKG-INFO` & `PythonToolsKit-1.2.4/PythonToolsKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.3
+Version: 1.2.4
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.3/PythonToolsKit.egg-info/SOURCES.txt` & `PythonToolsKit-1.2.4/PythonToolsKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.3/README.md` & `PythonToolsKit-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.3/setup.py` & `PythonToolsKit-1.2.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/sutools-0.1.1.tar.gz` & `tmp/sutools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sutools-0.1.1.tar", last modified: Sun Mar 19 17:50:05 2023, max compression
+gzip compressed data, was "sutools-0.1.2.tar", last modified: Sat Apr 29 02:35:02 2023, max compression
```

## Comparing `sutools-0.1.1.tar` & `sutools-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:50:05.974030 sutools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-19 17:49:42.000000 sutools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-19 17:50:05.974030 sutools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-03-19 17:49:42.000000 sutools-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-19 17:49:42.000000 sutools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 17:50:05.974030 sutools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-19 17:49:42.000000 sutools-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:50:05.970030 sutools-0.1.1/sutools/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-19 17:49:42.000000 sutools-0.1.1/sutools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-03-19 17:49:42.000000 sutools-0.1.1/sutools/cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-03-19 17:49:42.000000 sutools-0.1.1/sutools/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-19 17:49:42.000000 sutools-0.1.1/sutools/meta_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:50:05.970030 sutools-0.1.1/sutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-19 17:50:05.000000 sutools-0.1.1/sutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-19 17:50:05.000000 sutools-0.1.1/sutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 17:50:05.000000 sutools-0.1.1/sutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-19 17:50:05.000000 sutools-0.1.1/sutools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:50:05.974030 sutools-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-19 17:49:42.000000 sutools-0.1.1/tests/test_cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-03-19 17:49:42.000000 sutools-0.1.1/tests/test_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-19 17:49:42.000000 sutools-0.1.1/tests/test_meta_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-03-19 17:49:42.000000 sutools-0.1.1/tests/test_sutools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.207953 sutools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-29 02:34:38.000000 sutools-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-29 02:35:02.207953 sutools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-29 02:34:38.000000 sutools-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 02:34:38.000000 sutools-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:35:02.207953 sutools-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-29 02:34:38.000000 sutools-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.199952 sutools-0.1.2/sutools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-29 02:34:38.000000 sutools-0.1.2/sutools/meta_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.203953 sutools-0.1.2/sutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 02:35:02.000000 sutools-0.1.2/sutools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:35:02.207953 sutools-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_meta_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-29 02:34:38.000000 sutools-0.1.2/tests/test_sutools.py
```

### Comparing `sutools-0.1.1/LICENSE` & `sutools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/PKG-INFO` & `sutools-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sutools
-Version: 0.1.1
-Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
-Home-page: https://github.com/aastopher/sutools
-Author: Aaron Stopher
-Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
-Keywords: logs,logger,logging,cli,utils
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/sutools/badge/?version=latest)](https://sutools.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/aastopher/sutools/branch/master/graph/badge.svg?token=ZB0AX8D6JI)](https://codecov.io/gh/aastopher/sutools)
 [![PyPI version](https://badge.fury.io/py/sutools.svg)](https://badge.fury.io/py/sutools)
 [![DeepSource](https://deepsource.io/gh/aastopher/sutools.svg/?label=active+issues&show_trend=true&token=RVDa2T7M-E-YSg2DVFbr1ro-)](https://deepsource.io/gh/aastopher/sutools/?ref=repository-badge)
 
 ## Description
 
@@ -44,14 +29,28 @@
 @su.register
 def add(x : int, y : int):
     '''add two integers'''
     return x + y
 
 ```
 
+You can also register async functions, these will be executed using `asyncio.run()` given a valid coroutine function
+
+```python
+import sutools as su
+import asyncio
+
+@su.register
+async def delay_add(x : int, y : int):
+    '''add two integers after 1 sec'''
+    await asyncio.sleep(1)
+    return x + y
+    
+```
+
 **NOTE:** Adding type hinting to your functions enforces types in the cli and adds positional arg class identifiers in the help docs for the command.
 
 </br>
 
 ***
 
 ## CLI Usage Example
@@ -211,8 +210,8 @@
 
 **log output**
 ```
 16:16:34, 961 logger1 INFO 1 + 2 = 3
 16:16:34, 961 logger2 INFO 1 - 2 = -1
 ```
 
-***
+***
```

### Comparing `sutools-0.1.1/README.md` & `sutools-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: sutools
+Version: 0.1.2
+Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
+Home-page: https://github.com/aastopher/sutools
+Author: Aaron Stopher
+Project-URL: Documentation, https://sutools.readthedocs.io
+Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
+Keywords: logs,logger,logging,cli,utils
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Documentation Status](https://readthedocs.org/projects/sutools/badge/?version=latest)](https://sutools.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/aastopher/sutools/branch/master/graph/badge.svg?token=ZB0AX8D6JI)](https://codecov.io/gh/aastopher/sutools)
 [![PyPI version](https://badge.fury.io/py/sutools.svg)](https://badge.fury.io/py/sutools)
 [![DeepSource](https://deepsource.io/gh/aastopher/sutools.svg/?label=active+issues&show_trend=true&token=RVDa2T7M-E-YSg2DVFbr1ro-)](https://deepsource.io/gh/aastopher/sutools/?ref=repository-badge)
 
 ## Description
 
@@ -29,14 +45,28 @@
 @su.register
 def add(x : int, y : int):
     '''add two integers'''
     return x + y
 
 ```
 
+You can also register async functions, these will be executed using `asyncio.run()` given a valid coroutine function
+
+```python
+import sutools as su
+import asyncio
+
+@su.register
+async def delay_add(x : int, y : int):
+    '''add two integers after 1 sec'''
+    await asyncio.sleep(1)
+    return x + y
+    
+```
+
 **NOTE:** Adding type hinting to your functions enforces types in the cli and adds positional arg class identifiers in the help docs for the command.
 
 </br>
 
 ***
 
 ## CLI Usage Example
@@ -196,8 +226,8 @@
 
 **log output**
 ```
 16:16:34, 961 logger1 INFO 1 + 2 = 3
 16:16:34, 961 logger2 INFO 1 - 2 = -1
 ```
 
-***
+***
```

### Comparing `sutools-0.1.1/setup.py` & `sutools-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sutools",
-    version="0.1.1",
+    version="0.1.2",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["sutools"]),
     description="su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/sutools",
     project_urls={
+        "Documentation": "https://sutools.readthedocs.io",
         "Bug Tracker": "https://github.com/aastopher/sutools/issues",
     },
     keywords=['logs', 'logger', 'logging', 'cli', 'utils'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `sutools-0.1.1/sutools/__init__.py` & `sutools-0.1.2/sutools/__init__.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/sutools/cli_handler.py` & `sutools-0.1.2/sutools/cli_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import inspect, os, argparse, logging, sys
+import inspect, os, argparse, logging, sys, asyncio
 
 
 class CLI:
     """object designed for swift module CLI configuration"""
 
     def __init__(self, desc, logs, log_obj=None):
         """init top-level parser"""
@@ -123,14 +123,18 @@
             # unpack just the args and function
             func, arg_names = (
                 func_tup[0],
                 func_tup[1],
             )
             # collect given args from namespace
             args = [getattr(self.input, arg) for arg in arg_names]
+            
             # run function with given args and collect any returns
-            returned = func(*args)
+            if asyncio.iscoroutinefunction(func):
+                returned = asyncio.run(func(*args))
+            else:
+                returned = func(*args)
 
             # print return if not None
             if returned:
                 print(returned)
             sys.exit()  # exit the interpreter so the entire script is not run
```

### Comparing `sutools-0.1.1/sutools/log_handler.py` & `sutools-0.1.2/sutools/log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/sutools/meta_handler.py` & `sutools-0.1.2/sutools/meta_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/sutools.egg-info/PKG-INFO` & `sutools-0.1.2/sutools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.1.1
+Version: 0.1.2
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
+Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
 Keywords: logs,logger,logging,cli,utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -44,14 +45,28 @@
 @su.register
 def add(x : int, y : int):
     '''add two integers'''
     return x + y
 
 ```
 
+You can also register async functions, these will be executed using `asyncio.run()` given a valid coroutine function
+
+```python
+import sutools as su
+import asyncio
+
+@su.register
+async def delay_add(x : int, y : int):
+    '''add two integers after 1 sec'''
+    await asyncio.sleep(1)
+    return x + y
+    
+```
+
 **NOTE:** Adding type hinting to your functions enforces types in the cli and adds positional arg class identifiers in the help docs for the command.
 
 </br>
 
 ***
 
 ## CLI Usage Example
```

### Comparing `sutools-0.1.1/tests/test_cli_handler.py` & `sutools-0.1.2/tests/test_cli_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from unittest.mock import patch, Mock
-import sys, logging, argparse, pytest
+import sys, logging, argparse, pytest, asyncio
 from sutools import cli_handler, log_handler, meta_handler
 
 
 #### Fixtures
 @pytest.fixture
 def mock_atexit_register(monkeypatch):
     mock_atexit_register = Mock()
@@ -14,16 +14,16 @@
 #### Tests
 
 
 def test_cli_desc(capsys, monkeypatch):
     def func_test(
         test, test2: str, test3: str = "test", test4="test2", teest4: str = "test"
     ) -> str:
-        pass
-
+        pass # pass since we are only testing the function description
+    
     store = meta_handler.Bucket()
     store.add_func(func_test)
 
     expected = "Test CLI"
     cli_obj = cli_handler.CLI(expected, False)
     cli_obj.add_funcs(store.funcs)
 
@@ -153,15 +153,15 @@
 
     cli_obj = cli_handler.CLI("description", True, log_obj=log_obj)
     assert all(item in cli_obj.log.__dict__ for item in expected)
 
 
 def test_cli_add_funcs(capsys, monkeypatch):
     def func_test(x: int, y: int, c: str = "-") -> int:
-        pass
+        pass # pass since we are only testing the function is added to store
 
     expected = func_test.__name__
 
     namespace = argparse.Namespace(command="func_test", help=True, x=1, y=2, c="+")
 
     with patch(
         "sutools.cli_handler.argparse.ArgumentParser.parse_args", return_value=namespace
@@ -172,7 +172,51 @@
         cli_obj.add_funcs(store.funcs)
 
         monkeypatch.setattr(sys, "exit", lambda *args: None)
 
         cli_obj.parse()
 
     assert expected in cli_obj.parser.format_help()
+
+def test_async_func(capsys, monkeypatch, mock_atexit_register):
+    async def func_test():
+        await asyncio.sleep(0.1)
+        print('pass')
+
+    store = meta_handler.Bucket()
+    store.add_func(func_test)
+
+    log_obj = log_handler.Logger(
+        "test_logger",
+        list(store.funcs.keys()),
+        logging.INFO,
+        None,
+        None,
+        None,
+        None,
+        None,
+        None,
+        False,
+        logging.Formatter(
+            "%(asctime)s, %(msecs)d %(name)s %(levelname)s %(message)s",
+            datefmt="%H:%M:%S",
+        ),
+        logging.StreamHandler(sys.stdout),
+        stream=True,
+    )
+
+    cli_obj = cli_handler.CLI("description", False, log_obj=log_obj)
+    cli_obj.add_funcs(store.funcs)
+
+    monkeypatch.setattr(sys, "exit", lambda *args: None)
+
+    namespace = argparse.Namespace(command="func_test")
+
+    monkeypatch.setattr(
+        cli_handler.argparse.ArgumentParser, "parse_args", lambda self: namespace
+    )
+
+    cli_obj.parse()
+
+    captured = capsys.readouterr()
+
+    assert "pass" in captured.out
```

### Comparing `sutools-0.1.1/tests/test_log_handler.py` & `sutools-0.1.2/tests/test_log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/tests/test_meta_handler.py` & `sutools-0.1.2/tests/test_meta_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.1.1/tests/test_sutools.py` & `sutools-0.1.2/tests/test_sutools.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             fhandler=logging.FileHandler(
                 f"{mock_filepath}/{expected_filename}", "w", encoding="locale"
             ),
         )
 
         assert su.store.log is not None
         assert mock_os.path.join.call_args[0][0] == mock_filepath
-        assert mock_os.makedirs.called_once()
+        mock_os.makedirs.assert_called_once()
 
 
 def test_logger_cloggers(mock_os, mock_atexit_register):
     expected = ["logger1", "logger2", "logger3"]
 
     with patch("builtins.open", mock_open()):
         su.logger(
```


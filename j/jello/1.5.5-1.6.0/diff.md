# Comparing `tmp/jello-1.5.5.tar.gz` & `tmp/jello-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jello-1.5.5.tar", last modified: Sat Jan 14 22:37:26 2023, max compression
+gzip compressed data, was "jello-1.6.0.tar", last modified: Sat Apr 29 21:42:29 2023, max compression
```

## Comparing `jello-1.5.5.tar` & `jello-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-01-14 22:37:26.244868 jello-1.5.5/
--rw-r--r--   0 kelly      (501) staff       (20)     5451 2023-01-14 22:35:29.000000 jello-1.5.5/CHANGELOG
--rw-r--r--   0 kelly      (501) staff       (20)     1069 2023-01-12 03:25:15.000000 jello-1.5.5/LICENSE
--rw-r--r--   0 kelly      (501) staff       (20)       38 2023-01-12 03:25:15.000000 jello-1.5.5/MANIFEST.in
--rw-r--r--   0 kelly      (501) staff       (20)    15301 2023-01-14 22:37:26.245163 jello-1.5.5/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)    14803 2023-01-14 02:50:12.000000 jello-1.5.5/README.md
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-01-14 22:37:26.240290 jello-1.5.5/jello/
--rw-r--r--   0 kelly      (501) staff       (20)      228 2023-01-14 22:35:29.000000 jello-1.5.5/jello/__init__.py
--rw-r--r--   0 kelly      (501) staff       (20)       35 2023-01-14 02:50:12.000000 jello-1.5.5/jello/__main__.py
--rw-r--r--   0 kelly      (501) staff       (20)     6673 2023-01-14 02:50:12.000000 jello-1.5.5/jello/cli.py
--rw-r--r--   0 kelly      (501) staff       (20)    13103 2023-01-12 03:25:15.000000 jello-1.5.5/jello/dotmap.py
--rw-r--r--   0 kelly      (501) staff       (20)    17741 2023-01-14 22:35:29.000000 jello-1.5.5/jello/lib.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-01-14 22:37:26.243660 jello-1.5.5/jello.egg-info/
--rw-r--r--   0 kelly      (501) staff       (20)    15301 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)      324 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/SOURCES.txt
--rw-r--r--   0 kelly      (501) staff       (20)        1 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/dependency_links.txt
--rw-r--r--   0 kelly      (501) staff       (20)       41 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/entry_points.txt
--rw-r--r--   0 kelly      (501) staff       (20)       16 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/requires.txt
--rw-r--r--   0 kelly      (501) staff       (20)        6 2023-01-14 22:37:26.000000 jello-1.5.5/jello.egg-info/top_level.txt
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-01-14 22:37:26.244134 jello-1.5.5/man/
--rw-r--r--   0 kelly      (501) staff       (20)    12141 2023-01-12 03:25:15.000000 jello-1.5.5/man/jello.1
--rw-r--r--   0 kelly      (501) staff       (20)       73 2023-01-14 22:37:26.246287 jello-1.5.5/setup.cfg
--rwxr-xr-x   0 kelly      (501) staff       (20)      953 2023-01-14 22:35:29.000000 jello-1.5.5/setup.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-04-29 21:42:29.798651 jello-1.6.0/
+-rw-r--r--   0 kelly      (501) staff       (20)     5708 2023-04-29 21:40:46.000000 jello-1.6.0/CHANGELOG
+-rw-r--r--   0 kelly      (501) staff       (20)     1069 2023-01-12 03:25:15.000000 jello-1.6.0/LICENSE
+-rw-r--r--   0 kelly      (501) staff       (20)       38 2023-01-12 03:25:15.000000 jello-1.6.0/MANIFEST.in
+-rw-r--r--   0 kelly      (501) staff       (20)    15809 2023-04-29 21:42:29.798941 jello-1.6.0/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)    15311 2023-04-29 21:40:46.000000 jello-1.6.0/README.md
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-04-29 21:42:29.794380 jello-1.6.0/jello/
+-rw-r--r--   0 kelly      (501) staff       (20)      228 2023-04-29 21:40:46.000000 jello-1.6.0/jello/__init__.py
+-rw-r--r--   0 kelly      (501) staff       (20)       35 2023-01-14 02:50:12.000000 jello-1.6.0/jello/__main__.py
+-rw-r--r--   0 kelly      (501) staff       (20)     7707 2023-04-29 21:40:46.000000 jello-1.6.0/jello/cli.py
+-rw-r--r--   0 kelly      (501) staff       (20)    13103 2023-01-12 03:25:15.000000 jello-1.6.0/jello/dotmap.py
+-rw-r--r--   0 kelly      (501) staff       (20)    18486 2023-04-29 21:40:46.000000 jello-1.6.0/jello/lib.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-04-29 21:42:29.797652 jello-1.6.0/jello.egg-info/
+-rw-r--r--   0 kelly      (501) staff       (20)    15809 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)      324 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/SOURCES.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        1 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/dependency_links.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       41 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/entry_points.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       16 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/requires.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        6 2023-04-29 21:42:29.000000 jello-1.6.0/jello.egg-info/top_level.txt
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2023-04-29 21:42:29.798225 jello-1.6.0/man/
+-rw-r--r--   0 kelly      (501) staff       (20)    13048 2023-04-29 21:40:46.000000 jello-1.6.0/man/jello.1
+-rw-r--r--   0 kelly      (501) staff       (20)       73 2023-04-29 21:42:29.800042 jello-1.6.0/setup.cfg
+-rwxr-xr-x   0 kelly      (501) staff       (20)      953 2023-04-29 21:40:46.000000 jello-1.6.0/setup.py
```

### Comparing `jello-1.5.5/CHANGELOG` & `jello-1.6.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 jello changelog
 
+20230423 v1.6.0
+- Add the ability to directly use a JSON file or JSON Lines files as data input (`-f`)
+- Add the ability to load a query from a file (`-q`)
+- Add the empty data option (`-e`)
+- Fix user-defined functions in ~/.jelloconf initialization file
+
 20230114 v1.5.5
 - Fix schema output to ensure invalid variable names are enclosed in bracket notation
 - Fix to allow blank lines when slurping JSON Lines objects
 
 20220730 v1.5.4
 - Add `__main__.py` to package for `python -m jello` use cases
```

### Comparing `jello-1.5.5/LICENSE` & `jello-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jello-1.5.5/PKG-INFO` & `jello-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jello
-Version: 1.5.5
+Version: 1.6.0
 Summary: Filter JSON and JSON Lines data with Python syntax.
 Home-page: https://github.com/kellyjonbrazil/jello
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,22 +15,22 @@
 License-File: LICENSE
 
 [![Tests](https://github.com/kellyjonbrazil/jello/workflows/Tests/badge.svg?branch=master)](https://github.com/kellyjonbrazil/jello/actions)
 [![Pypi](https://img.shields.io/pypi/v/jello.svg)](https://pypi.org/project/jello/)
 
 >Built on `jello`:
 >- [Jello Explorer](https://github.com/kellyjonbrazil/jellex) (aka `jellex`) interactive TUI
->- `jello` [web demo](https://jello-web-demo.herokuapp.com/)
+>- `jello` [web demo](https://jello-web.onrender.com)
 
 # jello
 Filter JSON and JSON Lines data with Python syntax
 
 `jello` is similar to `jq` in that it processes JSON and JSON Lines data except `jello` uses standard python dict and list syntax.
 
-JSON or JSON Lines can be piped into `jello` (JSON Lines are automatically slurped into a list of dictionaries) and are available as the variable `_`. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
+JSON or JSON Lines can be piped into `jello` via STDIN or can be loaded from a JSON file or JSON Lines files (JSON Lines are automatically slurped into a list of dictionaries). Once loaded, the data is available as a python list or dictionary object named '`_`'. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
 
 For more information on the motivations for this project, see my [blog post](https://blog.kellybrazil.com/2020/03/25/jello-the-jq-alternative-for-pythonistas/).
 
 ## Install
 You can install `jello` via `pip`, via OS Package Repository, MSI installer for Windows, or by downloading the correct binary for your architecture and running it anywhere on your filesystem.
 
 ### Pip (macOS, linux, unix, Windows)
@@ -53,36 +53,46 @@
 
 > For more OS packages, see https://repology.org/project/jello/versions.
 
 See [Releases](https://github.com/kellyjonbrazil/jello/releases) on Github for MSI packages and binaries.
 
 ### Usage
 ```
-cat data.json | jello [OPTIONS] [QUERY]
+cat data.json | jello [OPTIONS] [QUERY | -q <query_file>]
+
+jello [OPTIONS] [QUERY | -q <query_file>] [-f <input_files>]
 ```
-`QUERY` is optional and can be most any valid python code. `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
+`QUERY` is optional and can be most any valid python code. Alternatively, a
+query file can be specified with `-q` to load the query from a file. Within the query, `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
 
 > Note: Reserved key names that cannot be accessed using dot notation can be accessed via standard python dictionary notation. (e.g. `_.foo["get"]` instead of `_.foo.get`)
 
 A simple query:
 ```bash
 cat data.json | jello _.foo
 ```
 or
 ```bash
-cat data.json | jello '_["foo"]'
+jello _.foo -f data.json
+```
+or
+```bash
+jello '_["foo"]' -f data.json
 ```
 
 #### Options
 - `-c` compact print JSON output instead of pretty printing
 - `-C` force color output even when using pipes (overrides `-m` and the `NO_COLOR` env variable)
+- `-e` empty data (don't process data from STDIN or file)
+- `-f` load input data from JSON file or JSON Lines files (must be the final option, if used)
 - `-i` initialize environment with a custom config file
 - `-l` lines output (suitable for bash array assignment)
 - `-m` monochrome output
 - `-n` print selected `null` values
+- `-q` load query from a file
 - `-r` raw output of selected strings (no quotes)
 - `-s` print the JSON schema in grep-able format
 - `-t` print type annotations in schema view
 - `-h` help
 - `-v` version info
 
 #### Simple Examples
```

### Comparing `jello-1.5.5/README.md` & `jello-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [![Tests](https://github.com/kellyjonbrazil/jello/workflows/Tests/badge.svg?branch=master)](https://github.com/kellyjonbrazil/jello/actions)
 [![Pypi](https://img.shields.io/pypi/v/jello.svg)](https://pypi.org/project/jello/)
 
 >Built on `jello`:
 >- [Jello Explorer](https://github.com/kellyjonbrazil/jellex) (aka `jellex`) interactive TUI
->- `jello` [web demo](https://jello-web-demo.herokuapp.com/)
+>- `jello` [web demo](https://jello-web.onrender.com)
 
 # jello
 Filter JSON and JSON Lines data with Python syntax
 
 `jello` is similar to `jq` in that it processes JSON and JSON Lines data except `jello` uses standard python dict and list syntax.
 
-JSON or JSON Lines can be piped into `jello` (JSON Lines are automatically slurped into a list of dictionaries) and are available as the variable `_`. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
+JSON or JSON Lines can be piped into `jello` via STDIN or can be loaded from a JSON file or JSON Lines files (JSON Lines are automatically slurped into a list of dictionaries). Once loaded, the data is available as a python list or dictionary object named '`_`'. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
 
 For more information on the motivations for this project, see my [blog post](https://blog.kellybrazil.com/2020/03/25/jello-the-jq-alternative-for-pythonistas/).
 
 ## Install
 You can install `jello` via `pip`, via OS Package Repository, MSI installer for Windows, or by downloading the correct binary for your architecture and running it anywhere on your filesystem.
 
 ### Pip (macOS, linux, unix, Windows)
@@ -37,36 +37,46 @@
 
 > For more OS packages, see https://repology.org/project/jello/versions.
 
 See [Releases](https://github.com/kellyjonbrazil/jello/releases) on Github for MSI packages and binaries.
 
 ### Usage
 ```
-cat data.json | jello [OPTIONS] [QUERY]
+cat data.json | jello [OPTIONS] [QUERY | -q <query_file>]
+
+jello [OPTIONS] [QUERY | -q <query_file>] [-f <input_files>]
 ```
-`QUERY` is optional and can be most any valid python code. `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
+`QUERY` is optional and can be most any valid python code. Alternatively, a
+query file can be specified with `-q` to load the query from a file. Within the query, `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
 
 > Note: Reserved key names that cannot be accessed using dot notation can be accessed via standard python dictionary notation. (e.g. `_.foo["get"]` instead of `_.foo.get`)
 
 A simple query:
 ```bash
 cat data.json | jello _.foo
 ```
 or
 ```bash
-cat data.json | jello '_["foo"]'
+jello _.foo -f data.json
+```
+or
+```bash
+jello '_["foo"]' -f data.json
 ```
 
 #### Options
 - `-c` compact print JSON output instead of pretty printing
 - `-C` force color output even when using pipes (overrides `-m` and the `NO_COLOR` env variable)
+- `-e` empty data (don't process data from STDIN or file)
+- `-f` load input data from JSON file or JSON Lines files (must be the final option, if used)
 - `-i` initialize environment with a custom config file
 - `-l` lines output (suitable for bash array assignment)
 - `-m` monochrome output
 - `-n` print selected `null` values
+- `-q` load query from a file
 - `-r` raw output of selected strings (no quotes)
 - `-s` print the JSON schema in grep-able format
 - `-t` print type annotations in schema view
 - `-h` help
 - `-v` version info
 
 #### Simple Examples
```

### Comparing `jello-1.5.5/jello/cli.py` & `jello-1.6.0/jello/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import signal
 import shutil
 import textwrap
 from textwrap import TextWrapper
 import jello
-from jello.lib import opts, load_json, pyquery, Schema, Json
+from jello.lib import opts, load_json, read_file, pyquery, Schema, Json
 
 
 def ctrlc(signum, frame):
     """exit with error on SIGINT"""
     sys.exit(1)
 
 
@@ -23,35 +23,40 @@
         return sys.stdin.read()
 
 
 def print_help():
     print(textwrap.dedent('''\
         jello:  query JSON at the command line with python syntax
 
-        Usage:  cat data.json | jello [OPTIONS] [QUERY]
+        Usage:  cat data.json | jello [OPTIONS] [QUERY | -q <query_file>]
+                jello [OPTIONS] [QUERY | -q <query_file>] [-f <input_files>]
 
                 -c   compact JSON output
                 -C   force color output even when using pipes (overrides -m)
+                -e   empty data (don't process data from STDIN or file)
+                -f   load input data from JSON file or JSON Lines files
                 -i   initialize environment with .jelloconf.py
                      located at ~ (linux) or %appdata% (Windows)
                 -l   output as lines suitable for assignment to a bash array
                 -m   monochrome output
                 -n   print selected null values
+                -q   load query from a file
                 -r   raw string output (no quotes)
                 -s   print the JSON schema in grep-able format
                 -t   print type annotations in schema view
                 -v   version info
                 -h   help
 
         Use '_' as the input data and use python dict and list bracket syntax
         or dot notation to filter the results and/or rebuild the output.
 
         Examples:
                 cat data.json | jello _.foo
-                cat data.json | jello '_["foo"]'
+                jello _.foo -f data.json
+                jello '_["foo"]' -f data.json
                 variable=($(cat data.json | jello -l _.foo))
     '''))
     sys.exit()
 
 
 def print_error(message):
     """print error messages to STDERR and quit with error code"""
@@ -116,32 +121,58 @@
         os.system('')
 
     if data is None:
         data = get_stdin()
 
     options = []
     long_options = {}
+    arg_section = ''  # can be query_file or data_files
 
     for arg in sys.argv[1:]:
-        if arg.startswith('-') and not arg.startswith('--'):
-            options.extend(arg[1:])
+        if arg == '-q':
+            arg_section = 'query_file'
+
+        elif arg == '-f':
+            data = ''
+            arg_section = 'data_files'
+
+        elif arg_section == 'query_file':
+            try:
+                query = read_file(arg)
+            except Exception as e:
+                print_error(f'jello:  Issue reading query file: {e}')
+            finally:
+                arg_section = ''
+
+        elif arg_section == 'data_files':
+            try:
+                data += '\n' + read_file(arg)
+            except Exception as e:
+                print_error(f'jello:  Issue reading data file: {e}')
+
+        elif arg.startswith('-') and not arg.startswith('--'):
+             options.extend(arg[1:])
+             arg_section = ''
 
         elif arg.startswith('--'):
             try:
                 k, v = arg[2:].split('=')
                 long_options[k] = int(v)
+                arg_section = ''
             except Exception:
                 print_help()
 
         else:
             query = arg
+            arg_section = ''
 
     opts.compact = opts.compact or 'c' in options
     opts.initialize = opts.initialize or 'i' in options
     opts.lines = opts.lines or 'l' in options
+    opts.empty = opts.empty or 'e' in options
     opts.force_color = opts.force_color or 'C' in options
     opts.mono = opts.mono or ('m' in options or bool(os.getenv('NO_COLOR')))
     opts.nulls = opts.nulls or 'n' in options
     opts.raw = opts.raw or 'r' in options
     opts.schema = opts.schema or 's' in options
     opts.types = opts.types or 't' in options
     opts.version_info = opts.version_info or 'v' in options
@@ -156,57 +187,57 @@
                     Author: {jello.AUTHOR}
                     Website: {jello.WEBSITE}
                     Copyright: {jello.COPYRIGHT}
                     License: {jello.LICENSE}
         '''))
         sys.exit()
 
-    if data is None:
-        print_error('jello:  missing piped JSON or JSON Lines data\n')
+    if data is None and not opts.empty:
+        print_error('jello:  Missing JSON or JSON Lines data via STDIN or file via -f option.\n')
+
+    if opts.empty:
+        data = '{}'
 
-    # only process if there is data
-    if data and not data.isspace():
+    # load the JSON or JSON Lines into a dict or list of dicts
+    try:
+        data = load_json(data)
+    except Exception as e:
+        print_exception(e, ex_type='JSON Load')
+
+    # Read .jelloconf.py (if it exists) and run the query
+    response = ''
+    try:
+        response = pyquery(data, query)
+    except Exception as e:
+        print_exception(e, data, query, ex_type='Query')
+
+    # reset opts.mono after pyquery since initialization in pyquery can change values
+    if opts.force_color:
+        opts.mono = False
+
+    # Create and print schema or JSON/JSON-Lines/Lines
+    output = ''
+    try:
+        if opts.schema:
+            schema = Schema()
+            output = schema.create_schema(response)
+
+            if not opts.mono and (sys.stdout.isatty() or opts.force_color):
+                schema.set_colors()
+                output = schema.color_output(output)
+
+        else:
+            json_out = Json()
+            output = json_out.create_json(response)
 
-        # load the JSON or JSON Lines into a dict or list of dicts
-        try:
-            data = load_json(data)
-        except Exception as e:
-            print_exception(e, ex_type='JSON Load')
-
-        # Read .jelloconf.py (if it exists) and run the query
-        response = ''
-        try:
-            response = pyquery(data, query)
-        except Exception as e:
-            print_exception(e, data, query, ex_type='Query')
-
-        # reset opts.mono after pyquery since initialization in pyquery can change values
-        if opts.force_color:
-            opts.mono = False
-
-        # Create and print schema or JSON/JSON-Lines/Lines
-        output = ''
-        try:
-            if opts.schema:
-                schema = Schema()
-                output = schema.create_schema(response)
-
-                if not opts.mono and (sys.stdout.isatty() or opts.force_color):
-                    schema.set_colors()
-                    output = schema.color_output(output)
-
-            else:
-                json_out = Json()
-                output = json_out.create_json(response)
-
-                if (not opts.mono and not opts.raw) and (sys.stdout.isatty() or opts.force_color):
-                    json_out.set_colors()
-                    output = json_out.color_output(output)
+            if (not opts.mono and not opts.raw) and (sys.stdout.isatty() or opts.force_color):
+                json_out.set_colors()
+                output = json_out.color_output(output)
 
-            print(output)
+        print(output)
 
-        except Exception as e:
-            print_exception(e, data, query, response, ex_type='Output')
+    except Exception as e:
+        print_exception(e, data, query, response, ex_type='Output')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `jello-1.5.5/jello/dotmap.py` & `jello-1.6.0/jello/dotmap.py`

 * *Files identical despite different names*

### Comparing `jello-1.5.5/jello/lib.py` & `jello-1.6.0/jello/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """jello - query JSON at the command line with python syntax"""
 
 import os
 import sys
+import types
 import ast
 import json
 import shutil
 from keyword import iskeyword
 from textwrap import TextWrapper
 from jello.dotmap import DotMap
 
@@ -39,14 +40,15 @@
 
 
 class opts:
     initialize = None
     version_info = None
     helpme = None
     compact = None
+    empty = None
     nulls = None
     raw = None
     lines = None
     force_color = None
     mono = None
     schema = None
     types = None
@@ -386,14 +388,17 @@
 
     for line in message_lines:
         if line == '':
             continue
         message = next_wrapper.fill(line)
         print(message, file=sys.stderr)
 
+def read_file(file_path):
+    with open(file_path, 'r') as f:
+        return f.read()
 
 def pyquery(data, query):
     """Sets options and runs the user's query."""
     output = None
 
     # read data into '_' variable
     # if data is a list of dictionaries, then need to iterate through and convert all dictionaries to DotMap
@@ -406,34 +411,44 @@
 
     else:
         _ = data
 
     # read initialization file to set colors, options, and user-defined functions
     jelloconf = ''
     conf_file = ''
+    jcnf_dict = {}
 
     if opts.initialize:
+        pyquery._ = _  # allows the data to be available to the initialization file
+
         if sys.platform.startswith('win32'):
-            conf_file = os.path.join(os.environ['APPDATA'], '.jelloconf.py')
+            conf_file_dir = os.environ['APPDATA']
         else:
-            conf_file = os.path.join(os.environ["HOME"], '.jelloconf.py')
+            conf_file_dir = os.environ["HOME"]
 
         try:
-            with open(conf_file, 'r') as f:
-                jelloconf = f.read()
+            conf_file = os.path.join(conf_file_dir, '.jelloconf.py')
+            jelloconf = read_file(conf_file)
+
+            # inject the data into the initialization module
+            conf_prepend = 'from jello.lib import pyquery as __q__\n'
+            conf_prepend += '_ = __q__._\n'
+            jelloconf = conf_prepend + jelloconf
+
+            # create and import the modified .jelloconf file as a normal module
+            jcnf = types.ModuleType('jcnf')
+            exec(jelloconf, jcnf.__dict__)
+            jcnf_dict = {f: getattr(jcnf, f) for f in dir(jcnf) if not f.startswith('__')}
 
         except FileNotFoundError:
             raise FileNotFoundError(f'-i used and initialization file not found: {conf_file}')
 
     warn_options = False
     warn_colors = False
 
-    i_block = ast.parse(jelloconf, mode='exec')
-    exec(compile(i_block, '<string>', mode='exec'))
-
     for option in [opts.compact, opts.raw, opts.lines, opts.nulls, opts.force_color, opts.mono, opts.schema, opts.types]:
         if not isinstance(option, bool) and option is not None:
             opts.compact = opts.raw = opts.lines = opts.nulls = opts.force_color = opts.mono = opts.schema = opts.types = False
             warn_options = True
 
     for color_config in [opts.keyname_color, opts.keyword_color, opts.number_color, opts.string_color]:
         valid_colors = ['black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'gray', 'brightblack',
@@ -453,18 +468,25 @@
     if warn_colors:
         valid_colors_string = ', '.join(valid_colors)
         warning_message([
             f'Colors must be set to one of: {valid_colors_string} in {conf_file}',
             'Unsetting all colors.'
         ])
 
+    # add any functions in initialization file to the scope
+    scope = {'_': _, 'os': os}
+    scope.update(jcnf_dict)
+
     # run the query
     block = ast.parse(query, mode='exec')
+
+    if len(block.body) < 1:
+        raise ValueError('No query found.')
+
     last = ast.Expression(block.body.pop().value)    # assumes last node is an expression
-    scope = {'_': _, 'os': os}
     exec(compile(block, '<string>', mode='exec'), scope)
     output = eval(compile(last, '<string>', mode='eval'), scope)
 
     # convert output back to normal dict
     if isinstance(output, list):
         output = [i.toDict() if isinstance(i, DotMap) else i for i in output]
```

### Comparing `jello-1.5.5/jello.egg-info/PKG-INFO` & `jello-1.6.0/jello.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jello
-Version: 1.5.5
+Version: 1.6.0
 Summary: Filter JSON and JSON Lines data with Python syntax.
 Home-page: https://github.com/kellyjonbrazil/jello
 Author: Kelly Brazil
 Author-email: kellyjonbrazil@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,22 +15,22 @@
 License-File: LICENSE
 
 [![Tests](https://github.com/kellyjonbrazil/jello/workflows/Tests/badge.svg?branch=master)](https://github.com/kellyjonbrazil/jello/actions)
 [![Pypi](https://img.shields.io/pypi/v/jello.svg)](https://pypi.org/project/jello/)
 
 >Built on `jello`:
 >- [Jello Explorer](https://github.com/kellyjonbrazil/jellex) (aka `jellex`) interactive TUI
->- `jello` [web demo](https://jello-web-demo.herokuapp.com/)
+>- `jello` [web demo](https://jello-web.onrender.com)
 
 # jello
 Filter JSON and JSON Lines data with Python syntax
 
 `jello` is similar to `jq` in that it processes JSON and JSON Lines data except `jello` uses standard python dict and list syntax.
 
-JSON or JSON Lines can be piped into `jello` (JSON Lines are automatically slurped into a list of dictionaries) and are available as the variable `_`. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
+JSON or JSON Lines can be piped into `jello` via STDIN or can be loaded from a JSON file or JSON Lines files (JSON Lines are automatically slurped into a list of dictionaries). Once loaded, the data is available as a python list or dictionary object named '`_`'. Processed data can be output as JSON, JSON Lines, bash array lines, or a grep-able schema.
 
 For more information on the motivations for this project, see my [blog post](https://blog.kellybrazil.com/2020/03/25/jello-the-jq-alternative-for-pythonistas/).
 
 ## Install
 You can install `jello` via `pip`, via OS Package Repository, MSI installer for Windows, or by downloading the correct binary for your architecture and running it anywhere on your filesystem.
 
 ### Pip (macOS, linux, unix, Windows)
@@ -53,36 +53,46 @@
 
 > For more OS packages, see https://repology.org/project/jello/versions.
 
 See [Releases](https://github.com/kellyjonbrazil/jello/releases) on Github for MSI packages and binaries.
 
 ### Usage
 ```
-cat data.json | jello [OPTIONS] [QUERY]
+cat data.json | jello [OPTIONS] [QUERY | -q <query_file>]
+
+jello [OPTIONS] [QUERY | -q <query_file>] [-f <input_files>]
 ```
-`QUERY` is optional and can be most any valid python code. `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
+`QUERY` is optional and can be most any valid python code. Alternatively, a
+query file can be specified with `-q` to load the query from a file. Within the query, `_` is the sanitized JSON from STDIN presented as a python dict or list of dicts. If `QUERY` is omitted then the original JSON input will simply be pretty printed. You can use dot notation or traditional python bracket notation to access key names.
 
 > Note: Reserved key names that cannot be accessed using dot notation can be accessed via standard python dictionary notation. (e.g. `_.foo["get"]` instead of `_.foo.get`)
 
 A simple query:
 ```bash
 cat data.json | jello _.foo
 ```
 or
 ```bash
-cat data.json | jello '_["foo"]'
+jello _.foo -f data.json
+```
+or
+```bash
+jello '_["foo"]' -f data.json
 ```
 
 #### Options
 - `-c` compact print JSON output instead of pretty printing
 - `-C` force color output even when using pipes (overrides `-m` and the `NO_COLOR` env variable)
+- `-e` empty data (don't process data from STDIN or file)
+- `-f` load input data from JSON file or JSON Lines files (must be the final option, if used)
 - `-i` initialize environment with a custom config file
 - `-l` lines output (suitable for bash array assignment)
 - `-m` monochrome output
 - `-n` print selected `null` values
+- `-q` load query from a file
 - `-r` raw output of selected strings (no quotes)
 - `-s` print the JSON schema in grep-able format
 - `-t` print type annotations in schema view
 - `-h` help
 - `-v` version info
 
 #### Simple Examples
```

### Comparing `jello-1.5.5/man/jello.1` & `jello-1.6.0/man/jello.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH jello 1 2022-06-26 1.5.3 "Jello JSON Filter"
+.TH jello 1 2022-06-26 1.6.0 "Jello JSON Filter"
 .SH NAME
 Jello \- Filter JSON and JSON Lines data with Python syntax
 .SH SYNOPSIS
 .PP
 Jello is similar to jq in that it processes JSON and
 JSON Lines data except jello uses standard python dict and
 list syntax.
@@ -12,23 +12,31 @@
 the variable `\fB_\fP`.
 Processed data can be output as JSON, JSON Lines, bash array lines, or a
 grep-able schema.
 .PP
 
 .SH USAGE
 
-cat data.json | jello [OPTIONS] [QUERY]
+.RS
+cat data.json | jello [OPTIONS] [QUERY | -q <query_file>]
+
+jello [OPTIONS] [QUERY | -q <query_file>] [-f <input_files>]
+.RE
 
 .fi
 .PP
-QUERY is optional and can be most any valid python code.
-`\fB_\fP` is the sanitized JSON from \fBSTDIN\fP presented as a python dict
-or list of dicts.
-If QUERY is omitted then the original JSON input will simply
+QUERY is optional and can be most any valid python code. Alternatively, a
+query file can be specified with `\fB-q\fP` to load the query from a file.
+Within the query, `\fB_\fP` is the sanitized JSON from \fBSTDIN\fP or the
+specified input file(s) (via the `\fB-f\fP` option) presented as a python
+dict or list of dicts.
+
+If QUERY or a query file is omitted then the original JSON input will simply
 be pretty printed.
+
 You can use dot notation or traditional python bracket notation to
 access key names.
 .RS
 .PP
 Note: Reserved key names that cannot be accessed using dot notation can
 be accessed via standard python dictionary notation.
 (e.g.
@@ -46,28 +54,42 @@
 or
 .IP
 .nf
 
 $ cat data.json | jello \[aq]_[\[dq]foo\[dq]]\[aq]
 
 .fi
+.PP
+or
+.IP
+.nf
+
+$ jello _.foo -f data.json
+
+.fi
 .SS Options
 .IP
 \fB-c\fP compact print JSON output instead of pretty printing
 .IP
 \fB-C\fP force color output even when using pipes (overrides \fB-m\fP and the \fBNO_COLOR\fP env variable)
 .IP
+\fB-e\fP empty data (don't process data from STDIN or file)
+.IP
+\fB-f\fP load input data from JSON file or JSON Lines files (must be the final option, if used)
+.IP
 \fB-i\fP initialize environment with a custom config file
 .IP
 \fB-l\fP lines output (suitable for bash array assignment)
 .IP
 \fB-m\fP monochrome output
 .IP
 \fB-n\fP print selected null values
 .IP
+\fB-q\fP load query from a file
+.IP
 \fB-r\fP raw output of selected strings (no quotes)
 .IP
 \fB-s\fP print the JSON schema in grep-able format
 .IP
 \fB-t\fP print type annotations in schema view
 .IP
 \fB-h\fP help
@@ -406,18 +428,17 @@
 .fi
 .SS Adding Functions
 .PP
 You can also add functions to your initialization file. For example, you could simplify \fBglom\fP use by adding the following function to \fB.jelloconf.py\fP:
 .IP
 .nf
 \f[C]
-def g(q, data=_):
+def g(query):
     import glom
-    return glom.glom(data, q)
-\f[R]
+    return glom.glom(_, query)
 .fi
 .PP
 Then you can use the following syntax to filter the JSON data:
 .IP
 .nf
 \f[C]
 $ jc -a | jello -i \[aq]g(\[dq]parsers.6.compatible\[dq])\[aq]
@@ -425,14 +446,37 @@
   \[dq]linux\[dq],
   \[dq]darwin\[dq],
   \[dq]cygwin\[dq],
   \[dq]win32\[dq],
   \[dq]aix\[dq],
   \[dq]freebsd\[dq]
 ]
+.fi
+.PP
+Or create names for commonly used queries:
+.IP
+.nf
+def darwin_compatible():
+    result = []
+    for entry in _.parsers:
+      if "darwin" in entry.compatible:
+        result.append(entry.name)
+    return result
+\f[R]
+.fi
+.PP
+Then use the predefined query like so:
+.IP
+.nf
+$ jc -a | jello -i \[aq]darwin_compatible()\[aq]
+[
+  \[dq]airport\[dq],
+  \[dq]airport-s\[dq],
+  \[dq]arp\[dq]
+]
 \f[R]
 .fi
 .SS Setting Custom Colors via Environment Variable
 .PP
 In addition to setting custom colors in the \fB.jelloconf.py\fP initialization file, you can also set them via the \fBJELLO_COLORS\fP environment variable. Any colors set in the environment variable will take precedence over any
 colors set in the initialization file.
 .PP
@@ -473,10 +517,10 @@
 
 .SH AUTHOR
 Kelly Brazil (kellyjonbrazil@gmail.com)
 
 https://github.com/kellyjonbrazil/jello
 
 .SH COPYRIGHT
-Copyright (c) 2020-2022 Kelly Brazil
+Copyright (c) 2020-2023 Kelly Brazil
 
 License: MIT License
```

### Comparing `jello-1.5.5/setup.py` & `jello-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='jello',
-    version='1.5.5',
+    version='1.6.0',
     author='Kelly Brazil',
     author_email='kellyjonbrazil@gmail.com',
     description='Filter JSON and JSON Lines data with Python syntax.',
     install_requires=[
         'Pygments>=2.4.2'
     ],
     license='MIT',
```


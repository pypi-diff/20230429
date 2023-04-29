# Comparing `tmp/TapisCL-ICICLE-0.0.31.tar.gz` & `tmp/TapisCL-ICICLE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.31.tar", last modified: Thu Apr 27 04:36:00 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.4.tar", last modified: Sat Apr 29 19:04:23 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.31.tar` & `TapisCL-ICICLE-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.572028 TapisCL-ICICLE-0.0.31/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/LICENSE
--rw-rw-rw-   0        0        0    44210 2023-04-27 04:36:00.570917 TapisCL-ICICLE-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.31/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.565819 TapisCL-ICICLE-0.0.31/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11005 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     9563 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5620 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     2059 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10683 2023-04-27 04:34:09.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    19575 2023-04-27 04:34:09.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.569881 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-04-27 04:35:02.000000 TapisCL-ICICLE-0.0.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 04:36:00.572028 TapisCL-ICICLE-0.0.31/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    45181 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-04-29 18:49:44.000000 TapisCL-ICICLE-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.328060 TapisCL-ICICLE-0.0.4/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0    11350 2023-04-29 18:56:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.334039 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3663 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/apps.py
+-rw-rw-rw-   0        0        0     2158 2023-04-29 18:35:45.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/baseWrappers.py
+-rw-rw-rw-   0        0        0     2459 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/files.py
+-rw-rw-rw-   0        0        0     5416 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/pods.py
+-rw-rw-rw-   0        0        0     2024 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/query.py
+-rw-rw-rw-   0        0        0     5022 2023-04-29 18:25:51.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     5353 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/systems.py
+-rw-rw-rw-   0        0        0     8464 2023-04-29 19:03:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/server.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.338635 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/args.py
+-rw-rw-rw-   0        0        0     9545 2023-04-29 18:02:05.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/decorators.py
+-rw-rw-rw-   0        0        0     2121 2023-04-29 18:26:16.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     6069 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/helpers.py
+-rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/logger.py
+-rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/schemas.py
+-rw-rw-rw-   0        0        0     1844 2023-04-29 17:29:42.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.342621 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    45181 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-29 18:41:37.000000 TapisCL-ICICLE-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.31/LICENSE` & `TapisCL-ICICLE-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.31/PKG-INFO` & `TapisCL-ICICLE-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.31
+Version: 0.0.4
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,26 +702,32 @@
 1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-**Full Terminal Interface:**
+#### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Command Line:**
+**Running Several Instances of Client**
+
+There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
+
+#### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
 **Scripting**
 
 Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
 
+### Known Issues
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
```

### Comparing `TapisCL-ICICLE-0.0.31/README.md` & `TapisCL-ICICLE-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,26 +12,32 @@
 1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-**Full Terminal Interface:**
+#### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Command Line:**
+**Running Several Instances of Client**
+
+There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
+
+#### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
 **Scripting**
 
 Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
 
+### Known Issues
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,54 +3,60 @@
 import argparse
 from argparse import SUPPRESS
 import sys
 import pyfiglet
 from getpass import getpass
 import os
 import time
-from pprint import pprint
-import json
-
 try:
-    from . import schemas
-    from . import socketOpts as SO
-    from . import helpers
-    from . import decorators
-    from . import args
+    from .utilities import schemas
+    from .utilities import socketOpts as SO
+    from .utilities import helpers
+    from .utilities import decorators
+    from .utilities import args
 except:
-    import schemas
-    import socketOpts as SO
-    import helpers
-    import decorators
-    import args
+    import utilities.schemas as schemas
+    import utilities.socketOpts as SO
+    import utilities.helpers as helpers
+    import utilities.decorators as decorators
+    import utilities.args as args
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, 'server.py')
 
 
 class CLI(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.Formatters):
     """
     Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
     """
     def __init__(self, IP: str, PORT: int):
+
         self.ip, self.port = IP, PORT
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
 
         # sets up connection with the server
         self.username, self.url = self.connect()
 
         # set up argparse
         self.parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=SUPPRESS)
         self.parser.add_argument('command_group')
 
+        self.message_handlers = {
+            'FormRequest':self.form_handler,
+            'AuthRequest':self.auth_handler,
+            'ConfirmationRequest':self.confirmation_handler,
+        }
+
         for parameters in args.Args.argparser_args.values():
             self.parser.add_argument(*parameters["args"], **parameters["kwargs"])
 
+        print(r"If you find any issues, please create a new issue here: https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues")
+
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
             os.system(f"pythonw {server_path}")
         else: # unix based
@@ -144,116 +150,124 @@
         for field in form:
             value = str(input(f"{field}: ")).strip()
             if not value:
                 value = None
             filled_form.update({field:value})
         return filled_form
 
-    def command_operator(self, kwargs: dict | list, exit_: int=0): 
+    def command_input_parser(self, kwargs: dict | list, exit_: int=0): 
         """
         parse arguments, handling bash and CLI input
         """
         if isinstance(kwargs, list): # check if the command input is from the CLI, or direct input
             kwargs = vars(self.parser.parse_args(kwargs)) 
         if not kwargs['command_group']:
             return False
         command = schemas.CommandData(kwargs = kwargs, exit_status = exit_)
         return command
     
+    def form_handler(self, response):
+        if not response.arguments_list:
+            form = self.expression_input()
+            filled_form = schemas.FormResponse(arguments_list=form)
+        else: 
+            form = self.fillout_form(response.arguments_list)
+            filled_form = schemas.FormResponse(arguments_list=form)
+        return filled_form
+
+    def auth_handler(self, response):
+        if response.secure_input or not response.requires_username:
+            username = self.username
+            password = getpass("Password: ")
+        else: 
+            username = input("Username: ")
+            password = getpass("Password: ")
+        filled_form = schemas.AuthData(username=username, password=password)
+        return filled_form
+    
+    def confirmation_handler(self, response):
+        print(response.message)
+        while True:
+            decision = str(input("(y/n)"))
+            if decision == 'y':
+                decision = True
+                break
+            elif decision == 'n':
+                decision = False
+                break
+            else:
+                print("Enter valid response")
+        filled_form = schemas.ResponseData(response_message=decision)
+        return filled_form
+    
     def special_forms_ops(self):
         """
         handle special form requests sent by the server
         """
         while True:
-            response = self.schema_unpack()
-            if response.schema_type == 'FormRequest' and not response.arguments_list:
-                form = self.expression_input()
-                filled_form = schemas.FormResponse(arguments_list=form)
-            elif response.schema_type == 'FormRequest':
-                form = self.fillout_form(response.arguments_list)
-                filled_form = schemas.FormResponse(arguments_list=form)
-            elif response.schema_type == 'AuthRequest':
-                if response.secure_input or not response.requires_username:
-                    username = self.username
-                    password = getpass("Password: ")
-                else: 
-                    username = input("Username: ")
-                    password = getpass("Password: ")
-                filled_form = schemas.AuthData(username=username, password=password)
-            elif response.schema_type == "ConfirmationRequest":
-                print(response.message)
-                while True:
-                    decision = str(input("(y/n)"))
-                    if decision == 'y':
-                        decision = True
-                        break
-                    elif decision == 'n':
-                        decision = False
-                        break
-                    else:
-                        print("Enter valid response")
-                filled_form = schemas.ResponseData(response_message=decision)
+            message = self.schema_unpack()
+            message_type = message.schema_type
+            if message_type in self.message_handlers.keys():
+                filled_form = self.message_handlers[message_type](message)
             else:
-                return response
+                return message
             self.json_send(filled_form.dict())
 
-    def print_response(self, response_message):
-        """
-        format response messages from the server
-        """
-        if type(response_message) == dict:
-            self.recursive_dict_print(response_message)
-        elif (type(response_message) == list or 
-             type(response_message) == tuple or 
-             type(response_message) == set):
-            for value in response_message:
-                print(value)
-        else:
-            print(response_message)
-
-    def main(self):
-        if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
-            try:
-                kwargs = self.parser.parse_args()
-            except:
-                print("Invalid Arguments")
-                os._exit(0)
-            kwargs = vars(kwargs)
-            command = self.command_operator(kwargs, exit_=1) # operate with args, send them over
-            self.json_send(command.dict())
-            response = self.special_forms_ops()
-            if response.schema_type == 'ResponseData':
-                self.print_response(response.response_message)
+    def environment_cli_response_stream_handler(self, response):
+        if response.schema_type == 'ResponseData' and response.exit_status: # if the command was a shutdown or exit, close the program
+            self.print_response(response.response_message)
+            os._exit(0)
+        elif response.schema_type == 'ResponseData':
+            if response.active_username:
+                self.username = response.active_username
+            if response.url:
+                self.url = response.url
+            self.print_response(response.response_message)
+
+    def terminal_cli(self):
+        try:
+            kwargs = self.parser.parse_args()
+        except:
+            print("Invalid Arguments")
             os._exit(0)
+        kwargs = vars(kwargs)
+        command = self.command_input_parser(kwargs, exit_=1) # operate with args, send them over
+        self.json_send(command.dict())
+        response = self.special_forms_ops()
+        if response.schema_type == 'ResponseData':
+            self.print_response(response.response_message)
+        os._exit(0)
 
+    def environment_cli(self):
         title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
         print(title)
         
         while True: # open the CLI if no arguments provided on startup
             try:
                 time.sleep(0.01)
                 kwargs = self.process_command(str(input(f"[{self.username}@{self.url}] "))) # ask for and process user input
                 try:
-                    command = self.command_operator(kwargs) # run operations
+                    command = self.command_input_parser(kwargs) # run operations
                 except:
                     continue
                 if not command:
                     continue
                 self.json_send(command.dict())
                 response = self.special_forms_ops()
-                if response.schema_type == 'ResponseData' and response.exit_status: # if the command was a shutdown or exit, close the program
-                    self.print_response(response.response_message)
-                    os._exit(0)
-                elif response.schema_type == 'ResponseData':
-                    self.print_response(response.response_message)
+                self.environment_cli_response_stream_handler(response)
             except KeyboardInterrupt:
                 pass # keyboard interrupts mess with the server, dont do it! it wont work anyway, hahahaha
             except WindowsError: # if connection error with the server (there wont be any connection errors)
                 print("[-] Connection was dropped. Exiting")
                 os._exit(0)
             except Exception as e: # if something else happens
                 print(e)
 
+    def main(self):
+        if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
+            self.terminal_cli()
+        self.environment_cli()
+
 
 if __name__ == "__main__":
     client = CLI(socket.gethostbyname(socket.gethostname()), 30000)
     client.main()
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/decorators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 DECORATORS
 These decorators are used in the tapisObjectWrappers.py file to standardize special functions. Allows for increased code reusability
 """
 import typing
-import socket
 import sys
 import time
 from functools import update_wrapper, partial
 try:
     from . import helpers
     from . import schemas
     from . import socketOpts
     from . import exceptions
 except:
-    import helpers
-    import schemas
-    import socketOpts
-    import exceptions
+    import utilities.helpers as helpers
+    import utilities.schemas as schemas
+    import utilities.socketOpts as socketOpts
+    import utilities.exceptions as exceptions
 
 
 class BaseRequirementDecorator(socketOpts.SocketOpts, helpers.OperationsHelper):
-    connection: typing.Optional[socket.socket] = None
     username: typing.Optional[str] = None
     password: typing.Optional[str] = None
     def __init__(self, func: typing.Callable):
         update_wrapper(self, func)
         self.function = func
         self.__code__ = func.__code__
         self.__doc__ = func.__doc__
@@ -48,85 +46,87 @@
 class RequiresForm(BaseRequirementDecorator):
     """
     This is for when you want to request separate input for specific command parameters instead of taking directly from the original command input (kwargs)
     Takes the parameters list of the function in question, filters out the ones that were not received from the original request message, sends another message 
     to request the unreceived parameters, and receives a message in response from the client to execute the function
     """
     def __call__(self, obj, *args, **kwargs):
-        if BaseRequirementDecorator.connection:
+        if kwargs['connection']:
             fields = list(helpers.get_parameters(self.function))
             for key, value in kwargs.items():
                 if value or value == False:
                     fields.remove(key)
             if not fields:
                 raise AttributeError(f"The decorated function {self.function} has no parameters.")
             form_request = schemas.FormRequest(arguments_list=fields)
-            self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
-            filled_form: schemas.FormResponse = self.schema_unpack_explicit(self.connection).arguments_list
+            self.json_send_explicit(kwargs['connection'], form_request.dict())
+            filled_form: schemas.FormResponse = self.schema_unpack_explicit(kwargs['connection']).arguments_list
             for key, value in filled_form.items():
                 kwargs[key] = value
 
         return self.function(obj, **kwargs)
 
 
 class RequiresExpression(BaseRequirementDecorator):
     """
     This is for when you have something like a Neo4j or postgres interface to add to the tapisObjectWrappers file. Writing a Neo4j query directly in a command is cumbersome, its much
     easier to do if you have a blank, multiline environment to write. This will send a request for an expression, if an expression parameter exists in the decorated function.
     The client will open a new interface to type the expression. This is then sent back and fed to the function
     """
     def __call__(self, obj, *args, **kwargs):
-        if BaseRequirementDecorator.connection:
+        if kwargs['connection']:
             fields = list(helpers.get_parameters(self.function))
             if 'expression' not in fields:
                 raise AttributeError(f"The function {self.function} does not contain an 'expression' parameter")
             form_request = schemas.FormRequest(arguments_list=[])
-            self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
-            filled_form: schemas.FormResponse = self.schema_unpack()
+            self.json_send_explicit(kwargs['connection'], form_request.dict())
+            filled_form: schemas.FormResponse = self.schema_unpack_explicit(connection=kwargs['connection'])
             kwargs['expression'] = filled_form.arguments_list
 
         return self.function(obj, **kwargs)
     
 
 class SecureInput(BaseRequirementDecorator):
     """
     Use this for functions where you need to hide input while typing into the cli. For instance, if you want to add a password to a service, as a user, but you dont actually
     want to authenticate. Checks if the decorated function has a password parameter, then requests secure input of a new password from the client
     """
     def __call__(self, obj, *args, **kwargs):
-        if BaseRequirementDecorator.connection:
+        if kwargs['connection']:
             fields = list(helpers.get_parameters(self.function))
             if 'password' in fields:
                 secure_input_request = schemas.AuthRequest(secure_input=True)
-                self.json_send_explicit(BaseRequirementDecorator.connection, secure_input_request.dict())
-                secure_input_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
+                self.json_send_explicit(kwargs['connection'], secure_input_request.dict())
+                secure_input_data: schemas.AuthData = self.schema_unpack_explicit(kwargs['connection'])
                 kwargs['password'] = secure_input_data.password
                 return self.function(obj, **kwargs)
             raise AttributeError(f"The function {self.function} does not contain a 'password' parameter to securely input")
         return self.function(obj, **kwargs)
 
 
 class Auth(BaseRequirementDecorator):
     """
     used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
     the client, and checks those credentials against the stored credentials in the server.
     """
     def __call__(self, obj, *args, **kwargs):
         no_username = False
-        if BaseRequirementDecorator.connection:
+        if kwargs['connection']:
             if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
                 return self.function(obj, **kwargs)
             fields = list(helpers.get_parameters(self.function))
             if kwargs['username']:
                 no_username = True
                 auth_request = schemas.AuthRequest(requires_username=False)
             else:
                 auth_request = schemas.AuthRequest()
-            self.json_send_explicit(BaseRequirementDecorator.connection, auth_request.dict())
-            auth_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
+            kwargs['connection'].setblocking(True)
+            self.json_send_explicit(kwargs['connection'], auth_request.dict())
+            auth_data: schemas.AuthData = self.schema_unpack_explicit(kwargs['connection'])
+            kwargs['connection'].setblocking(False)
             if 'username' in fields and 'password' in fields and not no_username:
                 kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
                 return self.function(obj, **kwargs)
             elif 'password' in fields and no_username:
                 kwargs['password'] = auth_data.password
             username, password = auth_data.username, auth_data.password
             if username != BaseRequirementDecorator.username:
@@ -138,33 +138,32 @@
 
 
 class NeedsConfirmation(BaseRequirementDecorator):
     """
     add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
     """
     def __call__(self, obj, *args, **kwargs):
-        if BaseRequirementDecorator.connection:
+        if kwargs['connection']:
             confirmation_request = schemas.ConfirmationRequest(message=f"YOU REQUESTED TO {self.function.__name__}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)")
-            self.json_send_explicit(BaseRequirementDecorator.connection, confirmation_request.dict())
-            confirmation_reply: schemas.ResponseData = self.schema_unpack_explicit(self.connection)
+            self.json_send_explicit(kwargs['connection'], confirmation_request.dict())
+            confirmation_reply: schemas.ResponseData = self.schema_unpack_explicit(kwargs['connection'])
             confirmed = confirmation_reply.response_message
             if not confirmed:
                 raise exceptions.NoConfirmationError(self.function)
         return self.function(obj, **kwargs)
 
     
 class DecoratorSetup:
     """
     for instantiation of the tapis wrappers, and the server, to set up decorators with user credentials and the socket connection. If you want to use the decorators in your class
     YOU WILL NEED TO USE THIS!
     """
-    def configure_decorators(self):
-        BaseRequirementDecorator.connection = self.connection
-        BaseRequirementDecorator.username = self.username
-        BaseRequirementDecorator.password = self.password
+    def configure_decorators(self, username, password):
+        BaseRequirementDecorator.username = username
+        BaseRequirementDecorator.password = password
     
 
 class AnimatedLoading:
     """
     Add this if you want to print a loading animation while a function is executing
     """
     def __init__(self, func: typing.Callable):
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,16 @@
 
 
 class HelpDoesNotExist(AttributeError):
     """
     raise error when the program tries to extract help information from a method, but help is not found
     """
     def __init__(self, command_name):
-        super().__init__(f"The command {command_name} has no help menu.\nMust include a docstring with @help: <help information>")
+        super().__init__(f"The command {command_name} has no help menu.\nMust include a docstring with @help: <help information>")
+
+
+class UnauthorizedAccessError(Exception):
+    """
+    raise error when an unauthorized IP tries to connect to the server
+    """
+    def __init__(self, ip):
+        super().__init__(f"DANGER! UNAUTHORIZED IP {ip} TRIED TO CONNECT TO THE SERVER. SOMEONE IS TRYING TO PIGGYBACK ON THE TAPIS APPLICATION, AND ATTEMPTING TO STEAL YOUR DATA.")
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import sys
 import threading
 import re
 try:
     from . import exceptions
     from . import args
 except:
-    import exceptions
-    import args
+    import utilities.exceptions as exceptions
+    import utilities.args as args
 
 
 command_parameters = args.Args.argparser_args
 
 
 def get_parameters(func):
     args = list(func.__code__.co_varnames[:func.__code__.co_argcount])
@@ -27,21 +27,17 @@
     """
     filters the kwargs received by the server to prevent an error from happening
     """
     def filter_kwargs(self, func: typing.Callable, kwargs: dict) -> dict:
         filtered = dict()
         variables = list(get_parameters(func))
         for arg in variables:
-            if arg in command_parameters: filtered.update({arg:kwargs[arg]})
+            if arg in command_parameters or arg == "connection": filtered.update({arg:kwargs[arg]})
             else: filtered.update({arg:None})
         return filtered
-
-    def print_dict(self, dict_):
-        for key, value in dict_.items():
-            print(f"{key}: {value}")
     
 
 class DynamicHelpUtility:
     """
     dynamically generate the help menu based on the doc  string and function arguments using .__doc__ and .__code__
     to generate helps for each command, iterate over the command map of the selected tapis wrapper object, and generate separate help menu for each
     """
@@ -146,14 +142,28 @@
                 for data in value:
                     print(("  " * (depth + 1)) + data)
             else: 
                 print(("  " * depth) + f"{key}: {str(value).strip()}")
         if depth == 1:
             print("\n")
 
+    def print_response(self, response_message):
+        """
+        format response messages from the server
+        """
+        if type(response_message) == dict:
+            self.recursive_dict_print(response_message)
+        elif (type(response_message) == list or 
+             type(response_message) == tuple or 
+             type(response_message) == set):
+            for value in response_message:
+                print(value)
+        else:
+            print(response_message)
+
 
 if __name__ == "__main__":
     class Silly:
         def z(self, y=True, x=False):
             return None
     x = OperationsHelper()
     v=Silly()
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 class ResponseData(BaseModel):
     """
     data from the server to the client with return data from commands, as well as errors
     """
     schema_type: str = 'ResponseData'
     response_message: Any
     exit_status: int = 0
+    url: str | None = None
+    active_username: str | None = None
 
 
 class FormRequest(BaseModel):
     """
     Request seperate input for some command parameters. If the arguments_list is empty, this will be interpreted as an expression request for something like neo4j
     """
     schema_type: str = 'FormRequest'
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/socketOpts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 try:
     from . import schemas
 except:
-    import schemas
+    import utilities.schemas as schemas
 
 
 schema_types: dict = {
         'CommandData':schemas.CommandData,
         'AuthData':schemas.AuthData,
         'StartupData':schemas.StartupData,
         'ResponseData':schemas.ResponseData,
@@ -25,19 +25,24 @@
         json_data = ""
         while True:
             try: 
                 json_data = json_data + connection.recv(1024).decode('utf-8') 
                 return json.loads(json_data) 
             except ValueError:
                 continue
+            except BlockingIOError:
+                continue
     
     def json_send_explicit(self, connection, data):
         json_data = json.dumps(data)
         connection.send(json_data.encode())
 
+    def schema_send_explicit(self, connection, data):
+        self.json_send_explicit(connection, data.dict())
+
     def schema_unpack_explicit(self, connection):
         data = self.json_receive_explicit(connection)
         schema_type = schema_types[data['schema_type']]
         return schema_type(**data)
 
     def json_receive(self) -> str | list | dict: # Receive and unpack json 
         return self.json_receive_explicit(self.connection)
```

### Comparing `TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.31
+Version: 0.0.4
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,26 +702,32 @@
 1. `pip install TapisCL-ICICLE`. Current version 0.0.24
 2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-**Full Terminal Interface:**
+#### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Command Line:**
+**Running Several Instances of Client**
+
+There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
+
+#### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
 **Scripting**
 
 Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
 
+### Known Issues
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
```

### Comparing `TapisCL-ICICLE-0.0.31/pyproject.toml` & `TapisCL-ICICLE-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.31"
+version = "0.0.4"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```


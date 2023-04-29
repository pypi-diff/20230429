# Comparing `tmp/miniagent-0.0.3-py3-none-any.whl.zip` & `tmp/miniagent-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,20 @@
-Zip file size: 14879 bytes, number of entries: 27
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-25 23:41 example/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-25 23:41 example/adaptee/__init__.py
--rw-rw-r--  2.0 unx     2195 b- defN 23-Apr-25 23:41 example/adaptee/tadaptees.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-25 23:41 example/adapter/__init__.py
--rw-rw-r--  2.0 unx      496 b- defN 23-Apr-25 23:41 example/adapter/payment_adapters.py
--rw-rw-r--  2.0 unx      418 b- defN 23-Apr-25 23:41 example/adapter/printer_adapters.py
--rw-rw-r--  2.0 unx     1093 b- defN 23-Apr-25 23:41 example/adapter/restserver_adapters.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-25 23:41 example/executer/__init__.py
--rw-rw-r--  2.0 unx     1623 b- defN 23-Apr-25 23:41 example/executer/purchase_card.py
--rw-rw-r--  2.0 unx     1216 b- defN 23-Apr-25 23:41 example/executer/refund_card.py
--rw-rw-r--  2.0 unx     1233 b- defN 23-Apr-25 23:41 example/executer/scheduler.py
--rw-rw-r--  2.0 unx       30 b- defN 23-Apr-25 23:41 example/model/__init__.py
--rw-rw-r--  2.0 unx      861 b- defN 23-Apr-25 23:41 example/model/tmodels.py
--rw-rw-r--  2.0 unx     2215 b- defN 23-Apr-26 03:04 miniagent/__init__.py
--rw-rw-r--  2.0 unx     1922 b- defN 23-Apr-25 23:41 miniagent/adapter.py
--rw-rw-r--  2.0 unx     3296 b- defN 23-Apr-25 23:41 miniagent/app_config.py
--rw-rw-r--  2.0 unx     1540 b- defN 23-Apr-25 23:41 miniagent/command_reciever.py
--rw-rw-r--  2.0 unx      852 b- defN 23-Apr-25 23:41 miniagent/common.py
--rw-rw-r--  2.0 unx      791 b- defN 23-Apr-25 23:41 miniagent/event_reciever.py
--rw-rw-r--  2.0 unx     3342 b- defN 23-Apr-25 23:41 miniagent/executer.py
--rw-rw-r--  2.0 unx      489 b- defN 23-Apr-25 23:41 miniagent/job_reciever.py
--rw-rw-r--  2.0 unx      275 b- defN 23-Apr-25 23:41 miniagent/models.py
--rw-rw-r--  2.0 unx     1063 b- defN 23-Apr-26 03:05 miniagent-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1705 b- defN 23-Apr-26 03:05 miniagent-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-26 03:05 miniagent-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-26 03:05 miniagent-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2212 b- defN 23-Apr-26 03:05 miniagent-0.0.3.dist-info/RECORD
-27 files, 28969 bytes uncompressed, 11301 bytes compressed:  61.0%
+Zip file size: 12482 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-29 08:47 miniadmin/__init__.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-29 08:47 miniadmin/admin.py
+-rw-rw-r--  2.0 unx     2556 b- defN 23-Apr-29 08:47 miniagent/__init__.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Apr-29 08:47 miniagent/adapter.py
+-rw-rw-r--  2.0 unx     3296 b- defN 23-Apr-29 08:47 miniagent/app_config.py
+-rw-rw-r--  2.0 unx     1540 b- defN 23-Apr-29 08:47 miniagent/command_reciever.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Apr-29 08:47 miniagent/common.py
+-rw-rw-r--  2.0 unx      791 b- defN 23-Apr-29 08:47 miniagent/event_reciever.py
+-rw-rw-r--  2.0 unx     3389 b- defN 23-Apr-29 08:47 miniagent/executer.py
+-rw-rw-r--  2.0 unx      528 b- defN 23-Apr-29 08:47 miniagent/job_reciever.py
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Apr-29 08:47 miniagent/message_reciever.py
+-rw-rw-r--  2.0 unx      275 b- defN 23-Apr-29 08:47 miniagent/models.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2321 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       71 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       20 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1442 b- defN 23-Apr-29 09:11 miniagent-0.0.4.dist-info/RECORD
+18 files, 24861 bytes uncompressed, 10126 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -1,44 +1,11 @@
-Filename: example/__init__.py
+Filename: miniadmin/__init__.py
 Comment: 
 
-Filename: example/adaptee/__init__.py
-Comment: 
-
-Filename: example/adaptee/tadaptees.py
-Comment: 
-
-Filename: example/adapter/__init__.py
-Comment: 
-
-Filename: example/adapter/payment_adapters.py
-Comment: 
-
-Filename: example/adapter/printer_adapters.py
-Comment: 
-
-Filename: example/adapter/restserver_adapters.py
-Comment: 
-
-Filename: example/executer/__init__.py
-Comment: 
-
-Filename: example/executer/purchase_card.py
-Comment: 
-
-Filename: example/executer/refund_card.py
-Comment: 
-
-Filename: example/executer/scheduler.py
-Comment: 
-
-Filename: example/model/__init__.py
-Comment: 
-
-Filename: example/model/tmodels.py
+Filename: miniadmin/admin.py
 Comment: 
 
 Filename: miniagent/__init__.py
 Comment: 
 
 Filename: miniagent/adapter.py
 Comment: 
@@ -57,26 +24,32 @@
 
 Filename: miniagent/executer.py
 Comment: 
 
 Filename: miniagent/job_reciever.py
 Comment: 
 
+Filename: miniagent/message_reciever.py
+Comment: 
+
 Filename: miniagent/models.py
 Comment: 
 
-Filename: miniagent-0.0.3.dist-info/LICENSE
+Filename: miniagent-0.0.4.dist-info/LICENSE
+Comment: 
+
+Filename: miniagent-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: miniagent-0.0.3.dist-info/METADATA
+Filename: miniagent-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: miniagent-0.0.3.dist-info/WHEEL
+Filename: miniagent-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: miniagent-0.0.3.dist-info/top_level.txt
+Filename: miniagent-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: miniagent-0.0.3.dist-info/RECORD
+Filename: miniagent-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miniagent/__init__.py

```diff
@@ -8,16 +8,17 @@
 import logging
 import logging.handlers
 from datetime import datetime
 from .app_config import AppConfig
 from .executer import ExecuterCaller
 from .command_reciever import CommandsReciever
 from .event_reciever import Command
+from .message_reciever import MessageReciever
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 #Load configuration
 configure = AppConfig(os.getcwd())
 configure.from_pyfile('config.py')
 
 #Set logging
 """
@@ -59,25 +60,34 @@
 scheduler.init_app(app)
 scheduler.start()
 
 #Executer
 executer = ExecuterCaller.instance(configure)
 
 #Command Reciever (Web url polling)
-reciever = None
+command_reciever = None
 if configure.get('COMMANDER_SERVER_URL'):
-    reciever = CommandsReciever(configure['COMMANDER_SERVER_URL'])
+    command_reciever = CommandsReciever(configure['COMMANDER_SERVER_URL'])
 
 #Table creation
 from . import models
 if configure.get('CUSTOM_MODELS_PATH'):
     mdl = import_module(configure['CUSTOM_MODELS_PATH'])
     cls_objs = [x for x in mdl.__dict__ if not x.startswith("_")]
     globals().update({k: getattr(mdl, k) for k in cls_objs})
 
 with app.app_context():
     db.create_all()
 
+#Kafka
+message_reciever = None
+if configure.get('EXECUTERS_BY_TOPIC') and configure.get('KAFKA_BOOTSTRAP_SERVERS'):
+    message_reciever = MessageReciever(
+        group_id = configure['AGENT_NAME'],
+        executers_by_topic = configure['EXECUTERS_BY_TOPIC']
+    )
+
+
 #Start scheduled jobs
 if configure.get('SCHEDULED_JOBS'):
     from .job_reciever import ScheduledJob
-    ScheduledJob(configure['SCHEDULED_JOBS'])
+    ScheduledJob(executer, configure['SCHEDULED_JOBS'])
```

## miniagent/adapter.py

```diff
@@ -17,14 +17,15 @@
 
         class_obj = getattr(package_module, class_name)
         
         if not issubclass(class_obj, Adapter):
             return None
 
         class_instance = class_obj()
+
         class_instance.set_adapter_name(class_path)
 
         return class_instance
 
 class Adapter(metaclass=abc.ABCMeta):
     
     def __init__(self):
@@ -43,14 +44,15 @@
 
     def set_adaptee(self, class_path: str):
         return self._create_adaptee(class_path)
 
     def _create_adaptee(self, class_path: str):
 
         if not class_path:
+            self.adaptee_name = ""
             return 1, "No Adaptee"
         
         package_name, class_name = split_class_path(class_path)
 
         try:
             package_module = import_module(package_name)
         except ImportError:
```

## miniagent/common.py

```diff
@@ -1,9 +1,10 @@
 import json
 import sys
+import os
 
 def split_class_path(class_path: str) -> tuple[str, str]:
 
     package_name = '.'.join(class_path.split('.')[:-1])
     class_name = class_path.split('.')[-1]
 
     return package_name, class_name
@@ -27,8 +28,8 @@
   def __getInstance(cls):
     return cls.__instance
 
   @classmethod
   def instance(cls, *args, **kargs):
     cls.__instance = cls(*args, **kargs)
     cls.instance = cls.__getInstance
-    return cls.__instance
+    return cls.__instance
```

## miniagent/executer.py

```diff
@@ -89,15 +89,15 @@
 
         adapters = dict()
 
         for param in sig.parameters.values():
 
             if param.name not in ['db', 'initial_param']:
                 dadapter = param.annotation.__module__ +'.'+param.annotation.__name__
-                dadaptee = self.default_adaptees[dadapter]
+                dadaptee = self.default_adaptees[dadapter] if self.default_adaptees.get(dadapter) else ""
                 adapter_instance = self._create_adapter(dadapter, dadaptee)
                 adapters[param.name] = adapter_instance
 
         print('execute_command adapters :',adapters)
 
         from . import app
```

## miniagent/job_reciever.py

```diff
@@ -1,20 +1,21 @@
 from datetime import datetime, timedelta
 from . import scheduler
 from .executer import ExecuterCaller
 
 class ScheduledJob:
 
-    def __init__(self, jobs: list) -> None:
+    def __init__(self, caller: ExecuterCaller, jobs: list) -> None:
 
+        self.caller = caller
         for job in jobs:
             self._run_job(job)
 
     def _run_job(self, job: dict) -> int:
 
         executer = job.pop('executer')
         scheduler.add_job(
-            func=ExecuterCaller.instance().execute_command,
+            func=self.caller.execute_command,
             args=[{'executer':executer}],
             **job
         )        
         return 1
```

## Comparing `miniagent-0.0.3.dist-info/LICENSE` & `miniagent-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miniagent-0.0.3.dist-info/METADATA` & `miniagent-0.0.4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagent
-Version: 0.0.3
+Version: 0.0.4
 Summary: PYPI tutorial package creation written by TeddyNote
 Home-page: https://github.com/tanminkwan/local-agent
 Author: tanminkwan
 Author-email: tanminkwan@gmail.com
 License: MIT
 Keywords: flask,sqlalchemy,scheduler
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,36 @@
 Miniagent is a multi-adaptable and lightweight application framework based on **Flask**.
 
 ## Installing
 
 Install and update using **pip**:
 `$ pip install -U miniagent`
 
+## Example code download
+
+Create an example project after installing miniagent
+
+`$ mini-project tanminkwan/local-agent test_project`
+
+Then test_project directory and files are created like the tree below.
+```
+└── test_project
+    ├── run.py
+    ├── config.py
+    └── myapp
+        ├── __init__.py
+        ├── adaptee.py
+        ├── adapter.py
+        ├── dbquery.py
+        ├── executer.py
+        └── model
+            ├── __init__.py
+            └── mymodels.py
+```
+
 ## A Simple Example
 
 There must be two files config.py and run.py in the base directory.
 ```
 # this is a sample config.py
 import os
 from datetime import datetime, timedelta
@@ -35,14 +57,15 @@
 base_dir = os.path.abspath(os.path.dirname(__file__))
 SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(base_dir, 'app.db')
 
 CUSTOM_MODELS_PATH = "example.model"
 
 DEFAULT_ADAPTEES =\
 {
+    "example.adapter.printer_adapters.PrinterAdapter":
     "example.adaptee.tadaptees.CardPrinterAdaptee",
     "example.adapter.payment_adapters.PaymentAdapter":
     "example.adaptee.tadaptees.CreditCardPaymentAdaptee",
 }
 SCHEDULED_JOBS =\
 [
     {
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


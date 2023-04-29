# Comparing `tmp/kegstand-0.2.1.tar.gz` & `tmp/kegstand-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.2.1.tar", max compression
+gzip compressed data, was "kegstand-0.3.0.tar", max compression
```

## Comparing `kegstand-0.2.1.tar` & `kegstand-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.2.1/LICENSE
--rw-r--r--   0        0        0     1151 2023-04-05 22:08:51.046908 kegstand-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      394 2023-04-05 09:20:02.898217 kegstand-0.2.1/src/kegstand/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-05 08:24:15.259719 kegstand-0.2.1/src/kegstand/api.py
--rw-r--r--   0        0        0     9910 2023-04-05 22:07:52.628549 kegstand-0.2.1/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1701 2023-04-05 09:02:45.455749 kegstand-0.2.1/src/kegstand/utils.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 kegstand-0.2.1/setup.py
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 kegstand-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1141 2023-04-29 19:34:52.696904 kegstand-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      394 2023-04-08 13:29:40.180072 kegstand-0.3.0/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-29 19:06:48.437560 kegstand-0.3.0/src/kegstand/api.py
+-rw-r--r--   0        0        0     9928 2023-04-08 13:23:20.126106 kegstand-0.3.0/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1255 2023-04-29 20:18:40.463405 kegstand-0.3.0/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.0/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.0/PKG-INFO
```

### Comparing `kegstand-0.2.1/LICENSE` & `kegstand-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.2.1/pyproject.toml` & `kegstand-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.2.1"
+version = "0.3.0"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
-repository = "https://github.com/jensroland/kegstand"
+repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
+#readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -21,15 +22,14 @@
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 aws-lambda-powertools = {extras = ["aws-sdk"], version = "^2.10.0"}
 pyjwt = "^2.1.0"
 python = "^3.9"
-tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.0"
 pytest = "^6.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `kegstand-0.2.1/src/kegstand/api.py` & `kegstand-0.3.0/src/kegstand/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,55 @@
     api_response,
     find_resource_modules,
 )
 from . import Logger
 
 logger = Logger()
 
-# Class KegstandApi provides a container for API resources and a method to add
+# Class RestApi provides a container for API resources and a method to add
 # resources to the API.
-class KegstandApi:
+class RestApi:
     def __init__(self, root: str = None):
         self.resources = []
         if root is not None:
             source_path = os.path.dirname(os.path.abspath(root))
             logger.info(f'Adding resources from {root} : source_path={source_path}')
             self.find_and_add_resources(source_path)
 
 
     def add_resource(self, resource):
         # Resource is a ApiResource object
         self.resources.append(resource)
 
 
-    def find_and_add_resources(self, source_root: str):
+    def find_and_add_resources(self, api_source_root: str):
         # Look through folder structure, importing and adding resources to the API.
         # Expects a folder structure like this:
         # api/
-        #   resources/
-        #       [resource_name]/
-        #           any.py which exposes a resource object named `api`
-        resource_module_folders = find_resource_modules(source_root)
+        #   [resource_name].py which exposes a resource object named `api`
+        resource_module_folders = find_resource_modules(api_source_root)
         for resource_module_folder in resource_module_folders:
             # Import the resource module
             resource_module = __import__(resource_module_folder['module_path'], fromlist=resource_module_folder['fromlist'])
             # Get the resource object from the module and add it to the API
             self.add_resource(getattr(resource_module, 'api'))
 
         return self.resources
 
 
     def export(self):
         # Export the API as a single Lambda-compatible handler function
         def handler(event, context):
             method = None
             for resource in self.resources:
-                if event['path'].startswith(resource.name):
+                if event['path'].startswith(resource.prefix):
                     method, params = resource.get_matching_route(event['httpMethod'], event['path'])
                     if method is not None:
                         break
 
-            # method = next(
-            #     (resource.get_matching_route(event['path']) for resource in self.resources), None
-            # )
-
             if method is None:
                 return api_response({'error': 'Not found'}, 404)
 
             # Call the method's handler function
             return method['handler'](params, event, context)
 
         return handler
```

### Comparing `kegstand-0.2.1/src/kegstand/decorators.py` & `kegstand-0.3.0/src/kegstand/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from .utils import api_response
 from . import Logger
 
 logger = Logger()
 
 # ApiResource provides a resource object that provides decorators for get, post, put, and delete
-# methods. The resource object also provides a name property that can be used to get the
-# resource's base name.
+# methods. The resource object also provides a prefix property that can be used to get the
+# resource's base prefix.
 class ApiResource:
-    def __init__(self, name: str, method_defaults: dict = None):
-        self.name = name
+    def __init__(self, prefix: str, method_defaults: dict = None):
+        self.prefix = prefix
         self.methods = []
         self.method_defaults = method_defaults or {}
 
     def get(self, route: str = '/', **kwargs):
         return self._method_decorator('GET', route, **{**self.method_defaults, **kwargs})
 
     def post(self, route: str = '/', **kwargs):
@@ -26,22 +26,22 @@
 
     def put(self, route: str = '/', **kwargs):
         return self._method_decorator('PUT', route, **{**self.method_defaults, **kwargs})
 
     def delete(self, route: str = '/', **kwargs):
         return self._method_decorator('DELETE', route, **{**self.method_defaults, **kwargs})
 
-    # Route contains the path to the resource method, relative to the resource's name
+    # Route contains the path to the resource method, relative to the resource's prefix
     # and may include dynamic segments (e.g. `/:id`).
     def _method_decorator(self, method: str, route: str, **kwargs):
         def decorator(func):
             @wraps(func)
             def wrapper(params, event, context):
                 if event['httpMethod'] != method:
-                    return api_response({'error': f'Method not allowed for name {self.name}'}, 405)
+                    return api_response({'error': f'Method not allowed for prefix {self.prefix}'}, 405)
 
                 try:
                     data = json.loads(event['body']) if event['body'] else {}
                 except json.JSONDecodeError:
                     return api_response({'error': 'Invalid JSON data provided'}, 400)
 
                 try:
@@ -84,15 +84,15 @@
                 except ApiError as e:
                     return e.to_api_response()
 
                 return api_response(response, 200)
 
             self.methods.append({
                 'route': route,
-                'full_route': self.name + route,
+                'full_route': self.prefix + route,
                 'method': method,
                 'handler': wrapper
             })
 
             return wrapper
         
         return decorator
```

### Comparing `kegstand-0.2.1/setup.py` & `kegstand-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `kegstand-0.2.1/PKG-INFO` & `kegstand-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.2.1
+Version: 0.3.0
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,9 +17,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aws-lambda-powertools[aws-sdk] (>=2.10.0,<3.0.0)
 Requires-Dist: pyjwt (>=2.1.0,<3.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
-Project-URL: Repository, https://github.com/jensroland/kegstand
+Project-URL: Repository, https://github.com/jensroland/kegstand-framework-python
```


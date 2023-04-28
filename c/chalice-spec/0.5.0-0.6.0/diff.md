# Comparing `tmp/chalice_spec-0.5.0.tar.gz` & `tmp/chalice_spec-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalice_spec-0.5.0.tar", max compression
+gzip compressed data, was "chalice_spec-0.6.0.tar", max compression
```

## Comparing `chalice_spec-0.5.0.tar` & `chalice_spec-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-02-13 23:04:42.862714 chalice_spec-0.5.0/LICENSE
--rw-r--r--   0        0        0     4231 2023-04-19 05:39:02.660502 chalice_spec-0.5.0/README.md
--rw-r--r--   0        0        0       97 2023-04-11 18:44:56.248615 chalice_spec-0.5.0/chalice_spec/__init__.py
--rw-r--r--   0        0        0     1966 2023-04-11 18:44:56.248858 chalice_spec-0.5.0/chalice_spec/blueprint.py
--rw-r--r--   0        0        0     5958 2023-04-19 05:39:02.660758 chalice_spec-0.5.0/chalice_spec/chalice.py
--rw-r--r--   0        0        0     2503 2023-04-11 18:44:56.249307 chalice_spec-0.5.0/chalice_spec/chalice_legacy.py
--rw-r--r--   0        0        0     7567 2023-04-19 05:39:02.660941 chalice_spec-0.5.0/chalice_spec/docs.py
--rw-r--r--   0        0        0     1485 2023-02-15 21:24:49.897244 chalice_spec-0.5.0/chalice_spec/pydantic.py
--rw-r--r--   0        0        0      631 2023-04-19 05:39:04.576939 chalice_spec-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5063 1970-01-01 00:00:00.000000 chalice_spec-0.5.0/setup.py
--rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 chalice_spec-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-02-13 23:04:42.862714 chalice_spec-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4199 2023-04-28 23:24:30.525468 chalice_spec-0.6.0/README.md
+-rw-r--r--   0        0        0       97 2023-04-11 18:44:56.248615 chalice_spec-0.6.0/chalice_spec/__init__.py
+-rw-r--r--   0        0        0     1966 2023-04-11 18:44:56.248858 chalice_spec-0.6.0/chalice_spec/blueprint.py
+-rw-r--r--   0        0        0     5953 2023-04-28 23:24:30.525812 chalice_spec-0.6.0/chalice_spec/chalice.py
+-rw-r--r--   0        0        0     2503 2023-04-11 18:44:56.249307 chalice_spec-0.6.0/chalice_spec/chalice_legacy.py
+-rw-r--r--   0        0        0     7567 2023-04-19 05:39:02.660941 chalice_spec-0.6.0/chalice_spec/docs.py
+-rw-r--r--   0        0        0     1485 2023-02-15 21:24:49.897244 chalice_spec-0.6.0/chalice_spec/pydantic.py
+-rw-r--r--   0        0        0      631 2023-04-28 23:24:37.628023 chalice_spec-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 chalice_spec-0.6.0/setup.py
+-rw-r--r--   0        0        0     4994 1970-01-01 00:00:00.000000 chalice_spec-0.6.0/PKG-INFO
```

### Comparing `chalice_spec-0.5.0/LICENSE` & `chalice_spec-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chalice_spec-0.5.0/README.md` & `chalice_spec-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 
 After:
 
 ```python
 from chalice_spec import ChaliceWithSpec, PydanticPlugin
 from apispec import APISpec
 
-spec = APISpec(chalice_app=app,
-               ...,
+spec = APISpec(...,
                plugins=[PydanticPlugin()])
 
 app = ChaliceWithSpec(app_name="hello_world", spec=spec)
 ```
 
 If you use
```

### Comparing `chalice_spec-0.5.0/chalice_spec/blueprint.py` & `chalice_spec-0.6.0/chalice_spec/blueprint.py`

 * *Files identical despite different names*

### Comparing `chalice_spec-0.5.0/chalice_spec/chalice.py` & `chalice_spec-0.6.0/chalice_spec/chalice.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,26 +33,30 @@
 
 class BlueprintWithSpec(Blueprint):
     """
     A Chalice Blueprint that has been augmented with chalice-spec to
     enable easy OpenAPI documentation.
     """
 
-    def __init__(self, import_name: str) -> None:
+    def __init__(self, import_name: str, tags=None) -> None:
         self._chalice_spec_docs = []
+        self._chalice_spec_tags = tags
         super(BlueprintWithSpec, self).__init__(import_name)
 
     def route(self, path: str, **kwargs: Any) -> Callable[..., Any]:
-        docs: Docs = kwargs.pop("docs", None)
+        def route_decorator(func):
+            docs: Docs = kwargs.pop("docs", None)
 
-        if docs:
             methods = [method.lower() for method in kwargs.get("methods", ["get"])]
-            self._chalice_spec_docs.append((path, methods, docs))
 
-        return super(BlueprintWithSpec, self).route(path, **kwargs)
+            self._chalice_spec_docs.append((path, methods, docs, func))
+
+            return super(BlueprintWithSpec, self).route(path, **kwargs)(func)
+
+        return route_decorator
 
 
 class ChaliceWithSpec(Chalice):
     """
     A Chalice app that has been augmented with chalice-spec to enable
     easy OpenAPI documentation.
 
@@ -74,95 +78,98 @@
                                            response=MyResponseModel)))
     def world():
         if app.current_request.method == "get":
             return {"an object": "that matches", "the schema": "APydantcModel"}
         # and so on!
     """
 
-    def __init__(self, app_name: str, spec: APISpec, generate_default_docs=False):
-        super().__init__(app_name)
+    def __init__(
+        self, app_name: str, spec: APISpec, generate_default_docs=False, **kwargs
+    ):
+        super().__init__(app_name, **kwargs)
 
         self.__spec = spec
         self.__generate_default_docs = generate_default_docs
 
+    def decorate(self, docs, path, methods, func, tags) -> None:
+        if docs is None and self.__generate_default_docs:
+            docs = default_docs_for_methods(methods)
+
+        if docs:
+            operations = docs.build_operations(self.__spec, methods)
+
+            # Infer path parameters
+            get_params = r"{([^}]+)}"
+            path_params = []
+            for param in re.findall(get_params, path):
+                path_params.append(
+                    {
+                        "in": "path",
+                        "name": param,
+                        "schema": {"type": "string"},
+                        "required": True,
+                    }
+                )
+
+            # Infer tags
+            for operation in operations:
+                if (
+                    "tags" not in operations[operation]
+                    or operations[operation]["tags"] is None
+                ):
+                    if tags:
+                        operations[operation]["tags"] = tags
+                    else:
+                        operations[operation]["tags"] = [
+                            "/" + path.lstrip("/").split("/", 1)[0]
+                        ]
+
+            # Infer summary and description from route docstrings
+            if func.__doc__:
+                split_docstring = trim_docstring(func.__doc__).split("\n", 1)
+                for operation in operations:
+                    if (
+                        "summary" not in operations[operation]
+                        or operations[operation]["summary"] is None
+                    ):
+                        operations[operation]["summary"] = split_docstring[0]
+                    if (
+                        "description" not in operations[operation]
+                        or operations[operation]["description"] is None
+                    ) and len(split_docstring) == 2:
+                        operations[operation]["description"] = split_docstring[
+                            1
+                        ].strip()
+
+            self.__spec.path(
+                path,
+                operations=operations,
+                summary=docs.summary,
+                parameters=path_params,
+            )
+
     def register_blueprint(
         self,
         blueprint: Union[Blueprint, BlueprintWithSpec],
         name_prefix: Optional[str] = None,
         url_prefix: Optional[str] = None,
     ) -> None:
         if isinstance(blueprint, BlueprintWithSpec):
-            for path, methods, docs in blueprint._chalice_spec_docs:
+            for path, methods, docs, func in blueprint._chalice_spec_docs:
                 path = (url_prefix if url_prefix else "") + path
 
-                if docs is None and self.__generate_default_docs:
-                    docs = default_docs_for_methods(methods)
-
-                if docs:
-                    operations = docs.build_operations(self.__spec, methods)
-                    self.__spec.path(path, operations=operations, summary=docs.summary)
+                self.decorate(docs, path, methods, func, blueprint._chalice_spec_tags)
 
         return super(ChaliceWithSpec, self).register_blueprint(
             blueprint, name_prefix=name_prefix, url_prefix=url_prefix
         )
 
     def route(self, path: str, **kwargs: Any) -> Callable[..., Any]:
         def route_decorator(func):
             docs: Docs = kwargs.pop("docs", None)
             methods = [method.lower() for method in kwargs.get("methods", ["get"])]
 
-            if docs is None and self.__generate_default_docs:
-                docs = default_docs_for_methods(methods)
-
-            if docs:
-                operations = docs.build_operations(self.__spec, methods)
-
-                # Infer path parameters
-                get_params = r"{([^}]+)}"
-                path_params = []
-                for param in re.findall(get_params, path):
-                    path_params.append(
-                        {
-                            "in": "path",
-                            "name": param,
-                            "schema": {"type": "string"},
-                            "required": True,
-                        }
-                    )
-
-                # Infer tags
-                for operation in operations:
-                    if (
-                        "tags" not in operations[operation]
-                        or operations[operation]["tags"] is None
-                    ):
-                        operations[operation]["tags"] = [
-                            "/" + path.lstrip("/").split("/", 1)[0]
-                        ]
-
-                # Infer summary and description from route docstrings
-                if func.__doc__:
-                    split_docstring = trim_docstring(func.__doc__).split("\n", 1)
-                    for operation in operations:
-                        if (
-                            "summary" not in operations[operation]
-                            or operations[operation]["summary"] is None
-                        ):
-                            operations[operation]["summary"] = split_docstring[0]
-                        if (
-                            "description" not in operations[operation]
-                            or operations[operation]["description"] is None
-                        ) and len(split_docstring) == 2:
-                            operations[operation]["description"] = split_docstring[
-                                1
-                            ].strip()
-
-                self.__spec.path(
-                    path,
-                    operations=operations,
-                    summary=docs.summary,
-                    parameters=path_params,
-                )
+            self.decorate(docs, path, methods, func, None)
 
             return super(ChaliceWithSpec, self).route(path, **kwargs)(func)
 
         return route_decorator
```

### Comparing `chalice_spec-0.5.0/chalice_spec/chalice_legacy.py` & `chalice_spec-0.6.0/chalice_spec/chalice_legacy.py`

 * *Files identical despite different names*

### Comparing `chalice_spec-0.5.0/chalice_spec/docs.py` & `chalice_spec-0.6.0/chalice_spec/docs.py`

 * *Files identical despite different names*

### Comparing `chalice_spec-0.5.0/chalice_spec/pydantic.py` & `chalice_spec-0.6.0/chalice_spec/pydantic.py`

 * *Files identical despite different names*

### Comparing `chalice_spec-0.5.0/pyproject.toml` & `chalice_spec-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chalice-spec"
-version = "0.5.0"
+version = "0.6.0"
 description = "Chalice x APISpec x Pydantic plug-ins"
 authors = ["Jake Wood <jake@testbox.com>"]
 repository = "https://github.com/TestBoxLab/chalice-spec"
 license = "MIT"
 keywords = ["Chalice", "AWS", "APIspec", "OpenAPI", "Pydantic"]
 readme = "README.md"
```

### Comparing `chalice_spec-0.5.0/setup.py` & `chalice_spec-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['apispec>=6.0.2,<7.0.0']
 
 setup_kwargs = {
     'name': 'chalice-spec',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Chalice x APISpec x Pydantic plug-ins',
-    'long_description': '# chalice-spec\n\n[![Python package](https://github.com/TestBoxLab/chalice-spec/actions/workflows/test.yml/badge.svg)](https://github.com/TestBoxLab/chalice-spec/actions/workflows/test.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Chalice × APISpec × Pydantic plug-ins**\n\nCombines the power of Chalice, APISpec, and Pydantic to make AWS Chalice apps easily documented\n\n## Installation\n\nFirst, add chalice-spec:\n\n```shell\npoetry add chalice_spec\n```\n\nWe consider Chalice, APISpec, and Pydantic "peer dependencies." We only include them as dev\ndependencies in our codebase, and you may need to install them in yours if you haven\'t\nalready.\n\n```shell\npoetry add chalice apispec pydantic\n```\n\n## Setup\n\nchalice-spec provides a subclass of the main `Chalice` class, called `ChaliceWithSpec`.\nHere is an example of how to get started:\n\nBefore:\n\n```python\nfrom chalice import Chalice\n\napp = Chalice(app_name="hello_world")\n```\n\nAfter:\n\n```python\nfrom chalice_spec import ChaliceWithSpec, PydanticPlugin\nfrom apispec import APISpec\n\nspec = APISpec(chalice_app=app,\n               ...,\n               plugins=[PydanticPlugin()])\n\napp = ChaliceWithSpec(app_name="hello_world", spec=spec)\n```\n\nIf you use\n\n```python\nChaliceWithSpec(..., generate_default_docs=True)\n```\n\nthe plugin will generate empty docs (with empty request and response schemas) for every endpoint that you\'ve defined in your app. This can be useful as a starting point / overview while developing.\n\n## Usage\n\nTo document your API, use your existing Pydantic models and add kwargs to Chalice decorators.\n\n**Before:**\n```python\n@app.route(\'/\', methods=["POST"])\ndef example():\n    body = MySchema.parse_obj(app.current_request.json_body)\n```\n\n**After:**\n```python\n@app.route(\'/\', methods=["POST"], docs=Docs(\n    post=Operation(request=MySchema)\n))\ndef example():\n    body = MySchema.parse_obj(app.current_request.json_body)\n```\n\nIf you have multiple methods supported, you may have something like:\n\n```python\n@app.route(\'/\', methods=["POST", "PUT"],\n           docs=Docs(\n               post=Operation(request=MyCreateSchema, response=MyReadSchema),\n               put=Operation(request=MyEditSchema, response=MyReadSchema)\n           )\ndef example():\n    # code goes here\n    pass\n```\n\n## Auto-Generation\n\n### Default Empty Docs\n\nIf you use:\n```python\nChalicePlugin(generate_default_docs=True)\n```\nthe plugin will generate empty docs (with empty request and response schemas) for every endpoint that you\'ve defined in your app. This can be useful as a starting point / overview while developing.\n\n### Path Parameters\n\nThese are inferred from the path itself. Any identifiers inside curly braces in a path is added as a string path parameter for that path. e.g. for the path `/users/{id}/friends/{f_id}`, the path parameters `id` and `f_id` will be added to the spec.\n\nTo disable this behaviour, define your own parameters or set them to an empty list:\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, parameters=[])\n```\n\n### Tags\n\nTags are used in things like Swagger to group endpoints into logical sets. If you don\'t supply any tags, chalice-spec will add a tag for each endpoint that is the first segment of the path. e.g. `/users`, `/users/{id}/friends`, and `/users/{id}/posts` will all be tagged with `users`.\n\nTo disable this behaviour, define `tags` in your operation (either with the tags you want, or an empty list):\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, tags=[])\n```\n\n### Summary and Description\n\nEndpoint summaries and descriptions are inferred from the route docstring. The first line of the docstring is used as the summary, and all other lines become the description:\n\n```python\n@app.route(\'/users/{id}\', methods=[\'GET\'], docs=Docs(response=UserSchema))\ndef get_user(id):\n    """\n    Retrieve a user object.\n    User\'s can\'t retrieve other users using this endpoint - only themselves.\n    """\n```\n\nTo disable this behaviour, you can define your own summary/description or set them to empty strings:\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, summary=\'\', description=\'\')\n```\n\n\n### API\n\n- [ ] TODO: this section coming soon!\n',
+    'long_description': '# chalice-spec\n\n[![Python package](https://github.com/TestBoxLab/chalice-spec/actions/workflows/test.yml/badge.svg)](https://github.com/TestBoxLab/chalice-spec/actions/workflows/test.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Chalice × APISpec × Pydantic plug-ins**\n\nCombines the power of Chalice, APISpec, and Pydantic to make AWS Chalice apps easily documented\n\n## Installation\n\nFirst, add chalice-spec:\n\n```shell\npoetry add chalice_spec\n```\n\nWe consider Chalice, APISpec, and Pydantic "peer dependencies." We only include them as dev\ndependencies in our codebase, and you may need to install them in yours if you haven\'t\nalready.\n\n```shell\npoetry add chalice apispec pydantic\n```\n\n## Setup\n\nchalice-spec provides a subclass of the main `Chalice` class, called `ChaliceWithSpec`.\nHere is an example of how to get started:\n\nBefore:\n\n```python\nfrom chalice import Chalice\n\napp = Chalice(app_name="hello_world")\n```\n\nAfter:\n\n```python\nfrom chalice_spec import ChaliceWithSpec, PydanticPlugin\nfrom apispec import APISpec\n\nspec = APISpec(...,\n               plugins=[PydanticPlugin()])\n\napp = ChaliceWithSpec(app_name="hello_world", spec=spec)\n```\n\nIf you use\n\n```python\nChaliceWithSpec(..., generate_default_docs=True)\n```\n\nthe plugin will generate empty docs (with empty request and response schemas) for every endpoint that you\'ve defined in your app. This can be useful as a starting point / overview while developing.\n\n## Usage\n\nTo document your API, use your existing Pydantic models and add kwargs to Chalice decorators.\n\n**Before:**\n```python\n@app.route(\'/\', methods=["POST"])\ndef example():\n    body = MySchema.parse_obj(app.current_request.json_body)\n```\n\n**After:**\n```python\n@app.route(\'/\', methods=["POST"], docs=Docs(\n    post=Operation(request=MySchema)\n))\ndef example():\n    body = MySchema.parse_obj(app.current_request.json_body)\n```\n\nIf you have multiple methods supported, you may have something like:\n\n```python\n@app.route(\'/\', methods=["POST", "PUT"],\n           docs=Docs(\n               post=Operation(request=MyCreateSchema, response=MyReadSchema),\n               put=Operation(request=MyEditSchema, response=MyReadSchema)\n           )\ndef example():\n    # code goes here\n    pass\n```\n\n## Auto-Generation\n\n### Default Empty Docs\n\nIf you use:\n```python\nChalicePlugin(generate_default_docs=True)\n```\nthe plugin will generate empty docs (with empty request and response schemas) for every endpoint that you\'ve defined in your app. This can be useful as a starting point / overview while developing.\n\n### Path Parameters\n\nThese are inferred from the path itself. Any identifiers inside curly braces in a path is added as a string path parameter for that path. e.g. for the path `/users/{id}/friends/{f_id}`, the path parameters `id` and `f_id` will be added to the spec.\n\nTo disable this behaviour, define your own parameters or set them to an empty list:\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, parameters=[])\n```\n\n### Tags\n\nTags are used in things like Swagger to group endpoints into logical sets. If you don\'t supply any tags, chalice-spec will add a tag for each endpoint that is the first segment of the path. e.g. `/users`, `/users/{id}/friends`, and `/users/{id}/posts` will all be tagged with `users`.\n\nTo disable this behaviour, define `tags` in your operation (either with the tags you want, or an empty list):\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, tags=[])\n```\n\n### Summary and Description\n\nEndpoint summaries and descriptions are inferred from the route docstring. The first line of the docstring is used as the summary, and all other lines become the description:\n\n```python\n@app.route(\'/users/{id}\', methods=[\'GET\'], docs=Docs(response=UserSchema))\ndef get_user(id):\n    """\n    Retrieve a user object.\n    User\'s can\'t retrieve other users using this endpoint - only themselves.\n    """\n```\n\nTo disable this behaviour, you can define your own summary/description or set them to empty strings:\n\n```python\nOperation(request=MySchema, response=MyOtherSchema, summary=\'\', description=\'\')\n```\n\n\n### API\n\n- [ ] TODO: this section coming soon!\n',
     'author': 'Jake Wood',
     'author_email': 'jake@testbox.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TestBoxLab/chalice-spec',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `chalice_spec-0.5.0/PKG-INFO` & `chalice_spec-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalice-spec
-Version: 0.5.0
+Version: 0.6.0
 Summary: Chalice x APISpec x Pydantic plug-ins
 Home-page: https://github.com/TestBoxLab/chalice-spec
 License: MIT
 Keywords: Chalice,AWS,APIspec,OpenAPI,Pydantic
 Author: Jake Wood
 Author-email: jake@testbox.com
 Requires-Python: >=3.7,<4.0
@@ -59,16 +59,15 @@
 
 After:
 
 ```python
 from chalice_spec import ChaliceWithSpec, PydanticPlugin
 from apispec import APISpec
 
-spec = APISpec(chalice_app=app,
-               ...,
+spec = APISpec(...,
                plugins=[PydanticPlugin()])
 
 app = ChaliceWithSpec(app_name="hello_world", spec=spec)
 ```
 
 If you use
```

